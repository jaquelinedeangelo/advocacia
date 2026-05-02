# 🎯 COLA RÁPIDA — Aula 1 (você usando GitHub Pages em vez de FTP)

> Imprima esta página ou deixe aberta numa segunda janela durante a aula.

---

## Tradução de comandos do instrutor

Quando o instrutor disser **uma das frases da coluna esquerda**, você faz **o que está na direita**:

| Instrutor diz... | Você faz no terminal |
|---|---|
| "Conecte no FTP" | Não precisa. Já está conectado pelo `git`. |
| "Suba para o FTP" / "Faça upload" | `git add . && git commit -m "atualiza" && git push` |
| "Veja o site no ar" | Abre `https://jaquelinedeangelo.github.io/advocacia/` |
| "Abra o cliente FTP" | Não precisa. Você só edita arquivos local + faz push. |
| "Apague o arquivo X do servidor" | `git rm <arquivo> && git commit -m "remove X" && git push` |
| "Crie a pasta paginas/captacao no servidor" | Cria local: `mkdir -p paginas/captacao` (já existe). Faz push depois. |

---

## Os 3 comandos sagrados (decorar)

Toda vez que você editar/criar arquivo e quiser publicar:

```bash
git add .
git commit -m "descricao do que mudou"
git push
```

📍 **Onde rodar:** dentro da pasta `~/Documents/escritorio-jaqueline/`. Pra entrar nela:
```bash
cd ~/Documents/escritorio-jaqueline
```

---

## Como saber se subiu

1. Espera ~30 segundos depois do `git push`
2. Abre `https://jaquelinedeangelo.github.io/advocacia/` no navegador
3. **Aperta Ctrl+F5** para forçar atualização (sem cache)
4. Se a alteração apareceu, ✅ subiu

---

## Se algo der errado

### "git: command not found"
Você precisa abrir o **Git Bash**, não o CMD. Procure "Git Bash" no menu Iniciar.

### Erro `failed to push`
Provavelmente alguém (ou você de outra máquina) editou o repositório. Rode:
```bash
git pull --rebase
git push
```

### "Estou perdida, instrutor falou X e não sei o que fazer"
Cola a frase exata do instrutor no Claude Code com:
> "Claude, o instrutor mandou fazer isso usando FTP. Como faço com GitHub Pages?"

---

## Variáveis importantes

```
Username:    jaquelinedeangelo
Repositório: jaquelinedeangelo/advocacia
Pasta local: ~/Documents/escritorio-jaqueline/
Site no ar:  https://jaquelinedeangelo.github.io/advocacia/
```

---

## Cheat sheet final em uma linha

> Editar arquivo → `git add . && git commit -m "msg" && git push` → esperar 30s → Ctrl+F5 no site → ✅
