# 🚀 Guia Rápido de Deploy

## GitHub Pages

### Passo a Passo:

1. **Criar repositório no GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Pollen website"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/pollen-1.git
   git push -u origin main
   ```

2. **Configurar GitHub Pages**
   - Acesse: `https://github.com/SEU-USUARIO/pollen-1/settings/pages`
   - Em "Source", selecione: `main` branch
   - Em "Folder", selecione: `/ (root)`
   - Clique em "Save"

3. **Acessar o site**
   - URL: `https://SEU-USUARIO.github.io/pollen-1/`
   - Pode levar alguns minutos para ficar disponível

### Importante:
- O arquivo `.nojekyll` já está incluído (evita processamento Jekyll)
- Certifique-se de que todos os arquivos estão na branch `main`

---

## Netlify

### Opção 1: Deploy via Interface Web

1. **Acesse**: https://app.netlify.com
2. **Clique em**: "Add new site" > "Import an existing project"
3. **Conecte** seu repositório GitHub
4. **Configure**:
   - Build command: (deixe vazio)
   - Publish directory: `/` (raiz)
5. **Clique em**: "Deploy site"

### Opção 2: Deploy via CLI

```bash
# Instalar Netlify CLI
npm install -g netlify-cli

# Login
netlify login

# Deploy
netlify deploy --prod
```

### Opção 3: Drag & Drop

1. Acesse: https://app.netlify.com/drop
2. Arraste a pasta do projeto
3. Aguarde o deploy automático

---

## Verificações Pós-Deploy

✅ Teste todas as páginas:
- Página principal (`index.html`)
- Política de privacidade (`privacy.html`)

✅ Verifique:
- Links de navegação funcionando
- Animações carregando corretamente
- Responsividade em mobile
- Formulário de contato funcionando

---

## Troubleshooting

### GitHub Pages não carrega CSS/JS
- Verifique se o arquivo `.nojekyll` está na raiz
- Certifique-se de que os caminhos dos arquivos estão corretos (relativos)

### Netlify mostra erro 404
- Verifique se `netlify.toml` está configurado corretamente
- Certifique-se de que `index.html` está na raiz

### Animações não funcionam
- Verifique o console do navegador para erros
- Certifique-se de que os CDNs estão carregando (GSAP, Three.js)

---

## URLs de Exemplo

Após o deploy, seu site estará disponível em:

- **GitHub Pages**: `https://SEU-USUARIO.github.io/pollen-1/`
- **Netlify**: `https://SEU-SITE.netlify.app` (ou domínio customizado)

---

## Próximos Passos

1. Configure um domínio customizado (opcional)
2. Adicione Google Analytics (se necessário)
3. Configure SSL/HTTPS (automático em ambos os serviços)
4. Otimize imagens (quando adicionar)

---

**Dúvidas?** Consulte o `README.md` para mais informações.

