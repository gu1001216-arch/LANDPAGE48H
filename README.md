# 🚀 Landing Page Estática - GitHub Pages

Uma landing page 100% estática, otimizada para venda de serviços de criação de sites com entrega em 48 horas.

## ✨ Características

✅ **100% Estático** - Nenhum servidor necessário
✅ **Um único arquivo HTML** - Fácil de gerenciar
✅ **Botão WhatsApp flutuante** - Com número direto
✅ **Gatilhos de conversão automáticos** - Detecta origem do tráfego
✅ **Mensagens personalizadas** - Google Ads, Facebook, Instagram
✅ **Totalmente responsivo** - Mobile, tablet, desktop
✅ **Otimizado para SEO** - Meta tags e estrutura semântica
✅ **Rápido e seguro** - Sem dependências externas

## 📱 Funcionalidades

### Botão WhatsApp
- Aparece após 2 segundos
- Animação de pulse após 10 segundos
- Número: +55 (48) 98421-7984
- Mensagens personalizadas por fonte de tráfego

### Gatilhos de Conversão
Detecta automaticamente a origem do tráfego:

**Google Ads:**
```
https://seu-site.com/?utm_source=google_ads&utm_medium=cpc&utm_campaign=nome
```
Mensagem: "Vi seu anúncio no Google..."

**Facebook:**
```
https://seu-site.com/?utm_source=facebook&utm_medium=social&utm_campaign=nome
```
Mensagem: "Vi seu anúncio no Facebook..."

**Instagram:**
```
https://seu-site.com/?utm_source=instagram&utm_medium=social&utm_campaign=nome
```
Mensagem: "Achei sua página no Instagram..."

## 🚀 Como Usar

### 1. Fazer Deploy no GitHub Pages

**Opção A: Repositório pessoal**
```bash
# 1. Crie um repositório chamado seu-username.github.io
# 2. Clone o repositório
git clone https://github.com/seu-username/seu-username.github.io.git
cd seu-username.github.io

# 3. Copie o arquivo index.html para a pasta
cp index.html .

# 4. Faça commit e push
git add index.html
git commit -m "Deploy landing page"
git push origin main

# 5. Sua página estará disponível em: https://seu-username.github.io
```

**Opção B: Repositório de projeto**
```bash
# 1. Crie um repositório qualquer (ex: landing-page)
git clone https://github.com/seu-username/landing-page.git
cd landing-page

# 2. Crie uma pasta docs e copie o arquivo
mkdir docs
cp index.html docs/

# 3. Faça commit e push
git add docs/index.html
git commit -m "Deploy landing page"
git push origin main

# 4. Nas configurações do repositório (Settings > Pages):
#    - Source: Deploy from a branch
#    - Branch: main
#    - Folder: /docs
#    - Sua página estará em: https://seu-username.github.io/landing-page
```

### 2. Personalizar o Site

**Alterar número de WhatsApp:**
Procure por `const phoneNumber = '5548984217984';` no arquivo e altere para seu número.

**Alterar cores:**
Procure pela seção `:root` no CSS e altere as variáveis:
```css
:root {
    --primary: #1e40af;      /* Azul profundo */
    --accent: #84cc16;       /* Verde-limão */
    /* ... outras cores */
}
```

**Alterar textos:**
Procure pelos textos no HTML e edite diretamente.

**Alterar imagens:**
As imagens estão hospedadas em CDN. Para usar suas próprias:
1. Hospede em Cloudinary, Imgix ou similar
2. Atualize as URLs no HTML

### 3. Configurar Google Analytics (Opcional)

Adicione este código antes de `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Substitua `GA_MEASUREMENT_ID` pelo seu ID do Google Analytics.

## 📊 Rastreamento de Conversão

O botão WhatsApp rastreia automaticamente cliques como eventos de conversão no Google Analytics.

Use os parâmetros UTM em suas campanhas:
- **utm_source**: google_ads, facebook, instagram
- **utm_medium**: cpc, social
- **utm_campaign**: nome-da-campanha

## 🎨 Estrutura do Site

1. **Header** - Logo e navegação
2. **Hero Section** - Título principal com CTA
3. **Features Section** - 3 benefícios principais
4. **Process Section** - 4 passos do processo
5. **CTA Section** - Formulário e WhatsApp
6. **Footer** - Informações de contato

## 📱 Responsividade

O site é totalmente responsivo e funciona perfeitamente em:
- Desktop (1024px+)
- Tablet (640px - 1024px)
- Mobile (< 640px)

## 🔒 Segurança

- Nenhum servidor necessário
- Nenhum armazenamento de dados
- Links de WhatsApp redirecionam para o app nativo
- Sem código backend exposto

## ⚡ Performance

- Arquivo único (sem requisições HTTP adicionais)
- CSS inline (sem requisições de folha de estilo)
- Imagens otimizadas em CDN
- Carregamento rápido

## 🐛 Troubleshooting

**Página não aparece após push:**
- Aguarde 5-10 minutos para GitHub processar
- Limpe o cache do navegador (Ctrl+Shift+Delete)
- Verifique as configurações de GitHub Pages

**Botão WhatsApp não funciona:**
- Verifique se o número está correto
- Teste em um dispositivo móvel
- Certifique-se de que WhatsApp está instalado

**Imagens não carregam:**
- Verifique se as URLs estão corretas
- Certifique-se de que os CDNs estão acessíveis

## 📞 Contato

**Número WhatsApp:** +55 (48) 98421-7984

## 📄 Licença

Este projeto é fornecido como está. Sinta-se livre para usar, modificar e distribuir.

---

**Criado em:** 10 de Fevereiro de 2026
**Versão:** 1.0.0
**Status:** Pronto para Produção ✅
