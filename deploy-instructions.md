# Instruções de Deploy - Portfólio HTML/CSS/JS Puro

## 🚀 Deploy no GitHub Pages (Recomendado)

### Passo 1: Criar Repositório
1. Acesse [GitHub](https://github.com) e faça login
2. Clique em "New repository"
3. Nome sugerido: `gabriel-portfolio-vanilla` ou `portfolio`
4. Marque como "Public"
5. Clique em "Create repository"

### Passo 2: Upload dos Arquivos
Você pode fazer upload de duas formas:

#### Opção A: Via Interface Web do GitHub
1. No repositório criado, clique em "uploading an existing file"
2. Arraste todos os arquivos do projeto para a área de upload
3. Escreva uma mensagem de commit: "Initial commit: Portfolio Steam-like"
4. Clique em "Commit changes"

#### Opção B: Via Git (se tiver instalado)
```bash
# No diretório do projeto
git init
git add .
git commit -m "Initial commit: Portfolio Steam-like"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPO.git
git push -u origin main
```

### Passo 3: Ativar GitHub Pages
1. No repositório, vá em "Settings"
2. Role até a seção "Pages"
3. Em "Source", selecione "Deploy from a branch"
4. Selecione "main" branch e "/ (root)"
5. Clique em "Save"
6. Aguarde alguns minutos e seu site estará disponível em:
   `https://SEU_USUARIO.github.io/NOME_DO_REPO`

## 🌐 Outras Opções de Deploy

### Netlify (Gratuito)
1. Acesse [Netlify](https://netlify.com)
2. Arraste a pasta do projeto para a área de deploy
3. Seu site estará online instantaneamente!
4. Para atualizações, conecte com seu repositório GitHub

### Vercel (Gratuito)
1. Acesse [Vercel](https://vercel.com)
2. Conecte com sua conta GitHub
3. Importe o repositório
4. Deploy automático a cada push!

### Surge.sh (Gratuito)
```bash
# Instalar Surge globalmente
npm install -g surge

# No diretório do projeto
surge

# Seguir as instruções no terminal
```

### Firebase Hosting (Gratuito)
```bash
# Instalar Firebase CLI
npm install -g firebase-tools

# No diretório do projeto
firebase login
firebase init hosting
firebase deploy
```

## 📱 Testando Localmente

### Método 1: Python (Recomendado)
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Acesse: http://localhost:8000
```

### Método 2: Node.js
```bash
# Instalar http-server globalmente
npm install -g http-server

# No diretório do projeto
http-server

# Acesse: http://localhost:8080
```

### Método 3: PHP
```bash
# Se tiver PHP instalado
php -S localhost:8000

# Acesse: http://localhost:8000
```

## 🔧 Customização Antes do Deploy

### Personalizando Informações
1. **Foto**: Substitua `assets/gabriel-photo.jpg` pela sua foto
2. **Informações pessoais**: Edite o HTML em `index.html`
3. **Links de contato**: Atualize os links na seção de contato
4. **Projetos**: Modifique os projetos de exemplo pelos seus reais
5. **Habilidades**: Ajuste as porcentagens das suas habilidades

### Personalizando Design
1. **Cores**: Edite as variáveis CSS em `:root` no `styles.css`
2. **Fontes**: Altere a importação do Google Fonts no HTML
3. **Layout**: Modifique o CSS para ajustar o layout
4. **Animações**: Adicione/remova animações no CSS e JavaScript

## 📊 SEO e Performance

### Otimizações Incluídas
- ✅ Meta tags para SEO
- ✅ Estrutura HTML semântica
- ✅ Alt text nas imagens
- ✅ Favicon personalizado
- ✅ CSS e JS otimizados
- ✅ Design responsivo

### Melhorias Adicionais
1. **Google Analytics**: Adicione o código de tracking
2. **Sitemap**: Crie um sitemap.xml
3. **Robots.txt**: Configure para SEO
4. **Open Graph**: Adicione meta tags para redes sociais

## 🎯 Domínio Personalizado

### GitHub Pages com Domínio Próprio
1. Compre um domínio (ex: gabrielvalente.dev)
2. No repositório, vá em Settings > Pages
3. Em "Custom domain", digite seu domínio
4. Configure o DNS do seu domínio:
   - Tipo: CNAME
   - Nome: www
   - Valor: SEU_USUARIO.github.io

### Netlify com Domínio Próprio
1. No painel do Netlify, vá em "Domain settings"
2. Clique em "Add custom domain"
3. Siga as instruções para configurar o DNS

## 🔒 HTTPS

Todos os serviços mencionados (GitHub Pages, Netlify, Vercel) oferecem HTTPS gratuito automaticamente.

## 📈 Monitoramento

### Google Analytics
Adicione este código antes do `</head>` no HTML:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Google Search Console
1. Acesse [Google Search Console](https://search.google.com/search-console)
2. Adicione sua propriedade (URL do site)
3. Verifique a propriedade
4. Envie o sitemap

## 🚨 Troubleshooting

### Site não carrega
- Verifique se o arquivo se chama `index.html`
- Confirme se está na branch correta (main)
- Aguarde alguns minutos após ativar o GitHub Pages

### Imagens não aparecem
- Verifique se os caminhos estão corretos
- Confirme se as imagens foram enviadas para o repositório
- Use caminhos relativos (ex: `assets/foto.jpg`)

### CSS/JS não funciona
- Verifique se os caminhos dos arquivos estão corretos
- Confirme se não há erros no console do navegador
- Teste localmente primeiro

## 📞 Suporte

Se tiver problemas:
1. Verifique a documentação do GitHub Pages
2. Teste localmente primeiro
3. Verifique o console do navegador para erros
4. Confirme se todos os arquivos foram enviados corretamente

---

🎮 **Boa sorte com seu portfólio Steam-like!**

