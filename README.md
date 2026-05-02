# Escritório Jaqueline de Angelo — Operação Digital

Esta é a pasta-mãe do escritório digital. O site está hospedado **grátis** no GitHub Pages.

🌐 **Site no ar:** https://jaquelinedeangelo.github.io/advocacia/  
📁 **Repositório:** https://github.com/jaquelinedeangelo/advocacia

---

## Como funciona o deploy (sem FTP)

A Aula 1 do curso ensina deploy com FTP (Hostinger). Você optou por GitHub Pages — é grátis e funciona igual de bom. Para publicar uma alteração, em vez de "subir via FTP", você faz:

```bash
cd ~/Documents/escritorio-jaqueline
git add .
git commit -m "descricao do que mudou"
git push
```

Em ~30 segundos o GitHub publica automático no endereço do site. Sem mexer em senha, sem cliente FTP.

⚡ **Atalho:** quando o instrutor disser *"agora suba para o FTP"*, você executa esses 3 comandos no terminal.

---

## Estrutura de pastas

```
escritorio-jaqueline/
├── index.html         ← página inicial atual (provisória — será substituída na Aula 1)
├── paginas/           ← outras páginas (HTML/CSS/JS)
│   ├── captacao/      ← landing page que captura leads
│   └── obrigado/      ← página pós-formulário (pixel, redirect)
│
├── supabase/          ← banco de dados e backend
│   └── schemas/       ← arquivos SQL com a estrutura das tabelas
│
├── videos/            ← seu conteúdo em vídeo (ignorados pelo git)
│   ├── brutos/        ← vídeos gravados pelo celular
│   └── editados/      ← vídeos finais
│
├── trafego/           ← campanhas Meta Ads (Aula 2)
├── whatsapp/          ← templates e fluxos do WhatsApp Business (Aula 3)
├── n8n/               ← automações
├── bi/                ← dashboards e relatórios
│
├── .env.example      ← modelo de variáveis de ambiente
├── .env              ← (criar a partir do .example, NUNCA vai pro GitHub)
├── .gitignore        ← arquivos que o Git ignora
├── requirements.txt  ← bibliotecas Python necessárias
└── README.md         ← este arquivo
```

---

## Como usar com o Claude Code

Abra esta pasta no Claude Code e peça em português natural. Exemplos já funcionando (skills instaladas):

- **"Cria a copy da minha página de captação"** → ativa a skill `copy-paginas`
- **"Monta o HTML/CSS dessa página"** → ativa a skill `frontend-design`
- **"Gera 10 hooks pros meus criativos do Instagram"** → ativa a skill `copy-criativos`

O Claude também já tem na memória as **regras OAB de publicidade** (`~/.claude/memory/regras_oab.md`), então toda copy gerada respeita o Provimento 205/2021.

---

## Próximos passos antes da Aula 1 (02/05/2026)

- [ ] Documentos físicos: CNPJ, OAB, RG, comprovante de endereço, cartão de crédito
- [ ] 1 vídeo bruto de 30-90s gravado pelo celular, salvo em `videos/brutos/`
- [ ] Conta Supabase confirmada (você já criou)
- [x] Hospedagem (GitHub Pages — grátis, já ativa)
- [x] Username GitHub profissional: `jaquelinedeangelo`
- [x] Site no ar: https://jaquelinedeangelo.github.io/advocacia/

---

## Em caso de erro

1. Tire screenshot do erro
2. Cole no Claude Code com a frase: "estou no curso ADV OPERADOR, dei esse erro"
3. Se não resolver em 10min, leve para o grupo de suporte
