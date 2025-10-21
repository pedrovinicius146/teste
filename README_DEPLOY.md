# Frontend pronto para deploy (Rope)

Arquivos atualizados para apontar para a API em:
https://rope-v2-production.up.railway.app

## O que foi feito
- Substituído `rope-v2-backend.up.railway.app` por `rope-v2-production.up.railway.app` nos arquivos `.js` e `.html` onde foi encontrado.
- Adicionado `vercel.json` para facilitar o deploy em **Vercel**.
- Empacotado em `frontend_deploy.zip` (este arquivo).

## Como fazer o deploy (duas opções rápidas)

### Opção A – Subir direto no Vercel (arrastar o zip)
1. Acesse https://vercel.com e faça login.
2. Clique em "New Project" → "Import" → "Upload" e arraste este ZIP.
3. Quando solicitado:
   - Framework/Template: escolha "Other".
   - Build Command: deixe em branco.
   - Output Directory: deixe em branco ou `/`.
4. Deploy — o site ficará disponível em uma URL vercel.app.

### Opção B – Usar GitHub + Vercel
1. Coloque o conteúdo desta pasta em um repositório GitHub (pasta raiz do repositório).
2. No Vercel, clique em "Import Project" e conecte o repositório.
3. Vercel detectará `vercel.json` e fará o deploy automaticamente.

## Teste local rápido
Você pode testar localmente com um servidor estático simples, por exemplo:
```
# usando npm (se tiver http-server)
npx http-server -c-1 .
# ou com Python 3
python -m http.server 8080
```
E acesse `http://localhost:8080`.

