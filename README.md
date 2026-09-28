# GMXURA OS v4 - Final

Sistema pessoal com login seguro, dashboard, cursos, kanban e segundo cérebro.

## 🚀 Deploy na Vercel via GitHub

1. Crie um repositório no GitHub (ex: `gmxura-os`)
2. Faça push deste projeto:
```bash
git init
git add .
git commit -m "GMXURA OS v4 - Final"
git branch -M main
git remote add origin https://github.com/SEUUSER/gmxura-os.git
git push -u origin main
```
3. Na Vercel: New Project > Import Git Repository
4. Framework: Other (Static)
5. Env Vars (opcional, mas recomendado):
   - `NEXT_PUBLIC_AUTH_USER` = gmxura
   - `NEXT_PUBLIC_AUTH_PASS` = 2014
6. Deploy!

## 🔐 Login
- Usuário: gmxura
- Senha: 2014
- Seguro: rate limit 5 tentativas + bloqueio 60s + sessão 24h

## 📁 Estrutura
```
├── index.html          # App principal (React + Tailwind, 100% funcional)
├── public/
│   ├── manifest.json   # PWA
│   ├── icon-192x192.png
│   ├── icon-512x512.png
│   ├── favicon-32x32.png
│   ├── gmxura_original_transparente.png # Logo sem fundo
│   └── icons/          # Todas variações da logo
├── vercel.json         # Headers de segurança + SPA rewrite
├── manifest.json       # PWA na raiz
├── package.json
└── README.md
```

## ✨ Funcionalidades
- **Login:** vidro branco frosted glass sobre fundo roxo premium, sem mostrar credenciais
- **Dashboard:** resumo + faturamento + CMD+K busca global
- **Cursos:** cada curso com cor personalizada (10 cores), checklist aulas com checkbox, YouTube embed, tempo estimado, certificados com Ver/Baixar (PDF/imagem base64)
- **Trabalho:** Kanban 4 colunas com cores fixas (A Fazer cinza, Em Andamento amarelo pulsante, Entregue roxo, Pago verde), drag & drop, faturamento mensal
- **Segundo Cérebro:** editor rico, [[links]], #tags, FAB captura rápida
- **Certificados:** aba dedicada lista todos
- **PWA:** instalável no celular

## 🎨 Logo
Logo original sem fundo branco: `public/gmxura_original_transparente.png`

## 🔧 Futuro
Conectar Supabase em Configurações > Nuvem para sincronizar PC e celular.
