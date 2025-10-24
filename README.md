# DialogaMente - Produção

🚀 **Deploy Automático Configurado!**

Este repositório contém a versão de produção do DialogaMente com deploy automático configurado para GitHub Pages e Netlify.

## 🌐 URLs de Acesso

- **GitHub Pages**: https://eupedrodiogo.github.io/DialogaMente-Producao/
- **Netlify**: (Configure o site no Netlify Dashboard)

## ⚡ Deploy Automático

### GitHub Pages
- ✅ Deploy automático a cada push na branch `main`
- ✅ Workflow configurado em `.github/workflows/deploy-github-pages.yml`
- ✅ Build otimizado com cache de dependências
- ✅ Análise de build e relatórios automáticos

### Netlify (Opcional)
- ✅ Workflow configurado em `.github/workflows/deploy-netlify.yml`
- ⚙️ Requer configuração de secrets no GitHub:
  - `NETLIFY_AUTH_TOKEN`
  - `NETLIFY_SITE_ID`

## 🔧 Configuração

### Secrets Necessários (Netlify)
Para habilitar o deploy no Netlify, adicione os seguintes secrets no GitHub:

1. Vá em **Settings** → **Secrets and variables** → **Actions**
2. Adicione:
   - `NETLIFY_AUTH_TOKEN`: Token de autenticação do Netlify
   - `NETLIFY_SITE_ID`: ID do site no Netlify

### GitHub Pages
O GitHub Pages está configurado automaticamente e não requer secrets adicionais.

## 📦 Estrutura do Projeto

```
DialogaMente-Producao/
├── .github/workflows/          # Workflows de CI/CD
│   ├── deploy-github-pages.yml # Deploy para GitHub Pages
│   └── deploy-netlify.yml      # Deploy para Netlify
├── deploy/                     # Arquivos de configuração de deploy
│   ├── _headers               # Headers de segurança e cache
│   ├── _redirects             # Redirects para SPA
│   ├── robots.txt             # SEO
│   ├── sitemap.xml            # Sitemap
│   └── manifest.json          # PWA manifest
├── src/                       # Código fonte (será sincronizado)
├── package.json               # Dependências e scripts
├── vite.config.ts             # Configuração do Vite
├── tailwind.config.ts         # Configuração do Tailwind
└── README.md                  # Este arquivo
```

## 🚀 Como Funciona

1. **Push para main**: Qualquer push para a branch `main` dispara os workflows
2. **Build automático**: O projeto é buildado automaticamente com `npm run build`
3. **Deploy simultâneo**: Deploy para GitHub Pages e Netlify (se configurado)
4. **Notificações**: Relatórios de build e deploy são gerados automaticamente

## 📊 Monitoramento

- **Build Status**: Verifique na aba "Actions" do GitHub
- **Deploy Logs**: Logs detalhados disponíveis nos workflows
- **Performance**: Análise de tamanho de build incluída

## 🔄 Sincronização

Este repositório será sincronizado automaticamente com o repositório principal do DialogaMente.

## 📝 Notas Importantes

- O base path está configurado para `/DialogaMente-Producao/` (GitHub Pages)
- Headers de segurança e cache estão otimizados
- PWA configurado com manifest.json
- SEO otimizado com robots.txt e sitemap.xml

---

**Status**: ✅ Deploy Automático Ativo
**Última atualização**: $(date)