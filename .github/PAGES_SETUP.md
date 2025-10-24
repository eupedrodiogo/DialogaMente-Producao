# Configuração do GitHub Pages

## ⚙️ Configuração Manual Necessária

Para ativar o GitHub Pages neste repositório, siga estes passos:

### 1. Acessar Configurações
1. Vá para o repositório: https://github.com/eupedrodiogo/DialogaMente-Producao
2. Clique em **Settings** (Configurações)
3. Role para baixo até a seção **Pages**

### 2. Configurar Source
1. Em **Source**, selecione: **GitHub Actions**
2. Isso permitirá que o workflow `.github/workflows/deploy-github-pages.yml` faça o deploy

### 3. Verificar Configuração
- ✅ Source: GitHub Actions
- ✅ Custom domain: (opcional)
- ✅ Enforce HTTPS: ✓ (recomendado)

### 4. Aguardar Deploy
Após a configuração:
1. O workflow será executado automaticamente
2. O site estará disponível em: https://eupedrodiogo.github.io/DialogaMente-Producao/
3. Verifique o status na aba **Actions**

## 🔍 Verificação

### URLs para Testar
- **Página Principal**: https://eupedrodiogo.github.io/DialogaMente-Producao/
- **Manifest**: https://eupedrodiogo.github.io/DialogaMente-Producao/manifest.json
- **Robots**: https://eupedrodiogo.github.io/DialogaMente-Producao/robots.txt
- **Sitemap**: https://eupedrodiogo.github.io/DialogaMente-Producao/sitemap.xml

### Status do Workflow
- Verifique em: https://github.com/eupedrodiogo/DialogaMente-Producao/actions
- O workflow `Deploy to GitHub Pages` deve estar verde ✅

## 🚨 Troubleshooting

### Se o deploy falhar:
1. Verifique os logs na aba Actions
2. Confirme que o GitHub Pages está configurado corretamente
3. Verifique se há erros de build no workflow

### Permissões
O workflow já está configurado com as permissões necessárias:
```yaml
permissions:
  contents: read
  pages: write
  id-token: write
```

---

**Próximos Passos**: Após configurar o GitHub Pages, o deploy será automático a cada push na branch `main`.