
# Metropole Data — Beta

Repositório para hospedar arquivos estáticos consumidos pelo app da Rádio Metrópole (MVP).

## Estrutura
```
/ (raiz)
├─ index.html
└─ v1/
   └─ programacao.json
```

## Como publicar no GitHub Pages
1. Crie um repositório no GitHub (ex.: `metropole-data`).
2. Envie estes arquivos para a branch `main`.
3. Vá em **Settings → Pages**.
4. Em **Build and deployment**, escolha **Source: Deploy from a branch**.
5. Selecione **Branch: main** e **/ (root)**. Salve.
6. Aguarde o link do Pages ficar ativo. Ex.: `https://SEU_USUARIO.github.io/metropole-data/`

### Endpoints resultantes
- Programação (v1): `https://SEU_USUARIO.github.io/metropole-data/v1/programacao.json`

> No futuro, quando tiver domínio próprio, use um subdomínio (ex.: `data.seu-dominio.com.br`) apontando via CNAME para o GitHub Pages e mantenha a versão (`/v1/`) para evoluir sem quebrar o app.

## Dicas
- Edite `v1/programacao.json` para atualizar a grade de programas (sem recompilar o app).
- Mantenha o campo `updated_at` atualizado.
- Se precisar de cache control mais fino, considere Netlify (com arquivo `_headers`).

---
Qualquer dúvida, me chama aqui. :)
