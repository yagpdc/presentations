# Driva · Apresentações

Catálogo de **demos de produto** navegáveis. Site estático puro (HTML/CSS/JS), sem build — deploy direto na Vercel.

## Estrutura

```
presentations/
├── index.html              # Home — catálogo de cards
└── base-ia-feature/
    └── index.html          # Demo "Copilot Ativo" → /base-ia-feature
```

## Como adicionar um novo produto

1. Crie uma pasta `nome-do-produto/` com um `index.html` dentro.
2. No `index.html` da raiz, copie um bloco `<a class="card live">` e aponte o `href` pra `./nome-do-produto/`.
3. A rota fica automática: `presentations.vercel.app/nome-do-produto`.

## Rodar local

Duplo-clique no `index.html` (abre no navegador). Tudo é standalone, sem servidor.

## Deploy (Vercel)

1. `vercel.com` → New Project → importar o repo `yagpdc/presentations`.
2. Framework Preset: **Other** (estático). Build/Output: deixar em branco.
3. Deploy. URLs:
   - `/` → home
   - `/base-ia-feature` → demo Copilot Ativo
