# 🚀 Guia de Deploy - JUPA 2025

## 📋 Pré-requisitos

### 1. Assets Necessários
Antes do deploy, certifique-se de ter os seguintes assets:

- [ ] **Vídeo MP4** para hero section (`/public/videos/jupa2025-hero.mp4`)
- [ ] **Logo oficial** em PNG/SVG (`/public/images/logo.png`)
- [ ] **Favicon** (`/public/favicon.ico`)
- [ ] **Imagem Open Graph** (`/public/og-image.jpg`)
- [ ] **Ícones PWA** (`/public/icon-192x192.png`, `/public/icon-512x512.png`)

### 2. Configuração de Ambiente
Crie o arquivo `.env.local`:

```env
# Google Forms
NEXT_PUBLIC_GOOGLE_FORMS_URL=https://docs.google.com/forms/d/e/1FAIpQLSd6-qyt4EDx_ZNSkQwl3atM88meRVLJfla4ptjg9nTgoiL4mg/viewform

# Analytics (opcional)
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX

# Upload de arquivos (se necessário)
NEXT_PUBLIC_UPLOAD_ENDPOINT=/api/upload
```

## 🌐 Deploy no Vercel (Recomendado)

### 1. Conectar Repositório
1. Acesse [vercel.com](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "New Project"
4. Importe o repositório `jupa-2025-site`

### 2. Configurar Variáveis de Ambiente
No painel do Vercel, adicione as variáveis:
- `NEXT_PUBLIC_GOOGLE_FORMS_URL`
- `NEXT_PUBLIC_GA_ID` (opcional)

### 3. Deploy Automático
- Push na branch `main` = Deploy automático
- Push em outras branches = Preview automático

## 🔧 Deploy Manual

### 1. Build Local
```bash
npm run build
```

### 2. Teste Local
```bash
npm start
```

### 3. Deploy
```bash
# Vercel CLI
npx vercel --prod

# Ou upload manual dos arquivos da pasta .next
```

## 📊 Monitoramento Pós-Deploy

### 1. Verificações Essenciais
- [ ] Site carrega corretamente
- [ ] Vídeo do hero funciona
- [ ] Formulário de inscrição funciona
- [ ] Links externos funcionam
- [ ] Responsividade em mobile
- [ ] Performance (Lighthouse)

### 2. Analytics
- Configure Google Analytics 4
- Monitore métricas de conversão
- Acompanhe tempo de carregamento

### 3. SEO
- Verifique metatags
- Teste Open Graph
- Valide structured data

## 🛠️ Manutenção

### 1. Atualização de Vagas
Para atualizar vagas disponíveis:
1. Edite `data/modalities.ts`
2. Altere `currentParticipants` para cada modalidade
3. Commit e push para atualizar automaticamente

### 2. Atualização de Conteúdo
- **FAQ**: Edite `data/faq.ts`
- **Informações do evento**: Edite `data/event.ts`
- **Downloads**: Edite `data/downloads.ts`

### 3. Backup
- Repositório GitHub serve como backup
- Vercel mantém histórico de deploys
- Documentos importantes em Google Drive

## 🚨 Troubleshooting

### Problemas Comuns

#### 1. Vídeo não carrega
- Verifique se o arquivo está em `/public/videos/`
- Confirme formato MP4
- Teste em diferentes navegadores

#### 2. Formulário não funciona
- Verifique URL do Google Forms
- Teste upload de arquivos
- Confirme variáveis de ambiente

#### 3. Performance lenta
- Otimize imagens
- Comprima vídeo
- Use CDN para assets

#### 4. SEO não funciona
- Verifique metatags
- Teste com Google Search Console
- Valide structured data

## 📞 Suporte

Para problemas técnicos:
- **WhatsApp**: (61) 98335-0225
- **Email**: gustavo@jupa2025.com.br
- **GitHub Issues**: Use o sistema de issues do repositório

## 🔄 Atualizações Futuras

### Próximas Funcionalidades
- [ ] Sistema de gestão de vagas em tempo real
- [ ] Área administrativa
- [ ] Notificações por email
- [ ] Sistema de pagamento integrado
- [ ] App mobile (PWA)

### Melhorias Planejadas
- [ ] Otimização de performance
- [ ] Testes automatizados
- [ ] Monitoramento avançado
- [ ] Backup automático

---

**Última atualização**: $(date)  
**Versão**: 1.0.0  
**Status**: Pronto para produção