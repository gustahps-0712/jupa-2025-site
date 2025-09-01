# JUPA 2025 - Site Oficial

Site oficial do JUPA 2025 - Jogos da União Presbiteriana de Adolescentes do Sínodo Bandeirante, Brasília.

## 🚀 Tecnologias Utilizadas

- **Next.js 14** - Framework React com App Router
- **TypeScript** - Tipagem estática
- **Tailwind CSS** - Estilização
- **Framer Motion** - Animações
- **React Hook Form** - Gerenciamento de formulários
- **React Dropzone** - Upload de arquivos
- **Lucide React** - Ícones

## 📋 Funcionalidades

### ✅ Implementadas
- [x] Design responsivo mobile-first
- [x] Hero section com vídeo em destaque
- [x] Sistema de navegação
- [x] Páginas: Home, Inscrições, Modalidades, Regulamento, Contato
- [x] Formulário de inscrição com upload de arquivos
- [x] Sistema de modalidades com contadores de vagas
- [x] FAQ interativo
- [x] Contador regressivo para fim das inscrições
- [x] Integração com Google Forms
- [x] SEO otimizado
- [x] Acessibilidade (WCAG AA)

### 🔄 Em Desenvolvimento
- [ ] Sistema de gestão de vagas em tempo real
- [ ] Área administrativa
- [ ] Analytics e monitoramento
- [ ] Testes automatizados

## 🛠️ Instalação e Execução

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn

### Instalação
```bash
# Clone o repositório
git clone https://github.com/gustahps-0712/jupa-2025-site.git

# Entre no diretório
cd jupa-2025-site

# Instale as dependências
npm install
# ou
yarn install
```

### Execução Local
```bash
# Modo desenvolvimento
npm run dev
# ou
yarn dev

# Acesse http://localhost:3000
```

### Build para Produção
```bash
# Build
npm run build
# ou
yarn build

# Iniciar servidor de produção
npm start
# ou
yarn start
```

## 📁 Estrutura do Projeto

```
jupa-2025-site/
├── app/                    # App Router (Next.js 14)
│   ├── globals.css        # Estilos globais
│   ├── layout.tsx         # Layout principal
│   ├── page.tsx           # Página inicial
│   ├── inscricoes/        # Página de inscrições
│   ├── modalidades/       # Página de modalidades
│   ├── regulamento/       # Página de regulamento
│   └── contato/           # Página de contato
├── components/            # Componentes React
│   ├── Hero.tsx          # Hero section com vídeo
│   ├── Navigation.tsx    # Navegação principal
│   ├── Footer.tsx        # Rodapé
│   ├── QuickInfo.tsx     # Informações rápidas
│   ├── Modalities.tsx    # Lista de modalidades
│   ├── RegistrationForm.tsx # Formulário de inscrição
│   ├── FAQ.tsx           # Perguntas frequentes
│   └── CountdownTimer.tsx # Contador regressivo
├── data/                 # Dados estáticos
│   ├── event.ts         # Informações do evento
│   ├── modalities.ts    # Modalidades esportivas
│   ├── faq.ts          # Perguntas frequentes
│   └── downloads.ts    # Arquivos para download
├── types/               # Definições TypeScript
│   └── index.ts        # Tipos principais
└── public/             # Arquivos estáticos
    ├── images/         # Imagens
    └── videos/         # Vídeos
```

## 🎨 Identidade Visual

### Paleta de Cores
- **Primária**: Laranja (#f97316) - Baseada no logo oficial
- **Secundária**: Cinza (#64748b) - Para textos e elementos neutros
- **Acento**: Amarelo (#eab308) - Para destaques
- **Fundo**: Cinza escuro (#111827) - Para contraste

### Tipografia
- **Fonte Principal**: Inter (Google Fonts)
- **Pesos**: 300, 400, 500, 600, 700, 800, 900

## 📱 Responsividade

O site foi desenvolvido com abordagem mobile-first:
- **Mobile**: < 768px
- **Tablet**: 768px - 1024px  
- **Desktop**: > 1024px

## 🔧 Configuração de Ambiente

### Variáveis de Ambiente
Crie um arquivo `.env.local` na raiz do projeto:

```env
# Google Forms
NEXT_PUBLIC_GOOGLE_FORMS_URL=https://docs.google.com/forms/d/e/1FAIpQLSd6-qyt4EDx_ZNSkQwl3atM88meRVLJfla4ptjg9nTgoiL4mg/viewform

# Analytics (opcional)
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX

# Upload de arquivos (configurar conforme necessário)
NEXT_PUBLIC_UPLOAD_ENDPOINT=/api/upload
```

## 🚀 Deploy

### Vercel (Recomendado)
1. Conecte o repositório ao Vercel
2. Configure as variáveis de ambiente
3. Deploy automático a cada push na branch main

### Netlify
1. Conecte o repositório ao Netlify
2. Configure o build command: `npm run build`
3. Configure o publish directory: `.next`

### Outros Provedores
O projeto é compatível com qualquer provedor que suporte Next.js.

## 📊 Monitoramento

### Analytics
- Google Analytics 4 (configurável)
- Métricas de performance
- Tracking de conversões

### Logs
- Logs de erro automáticos
- Monitoramento de uptime
- Alertas de performance

## 🧪 Testes

### Checklist de QA
- [ ] Teste em Chrome, Firefox, Safari, Edge
- [ ] Teste em dispositivos móveis (iOS/Android)
- [ ] Teste de responsividade
- [ ] Teste de upload de arquivos
- [ ] Teste de formulários
- [ ] Teste de acessibilidade
- [ ] Teste de performance
- [ ] Teste de SEO

## 📞 Suporte

Para dúvidas técnicas ou suporte:
- **Contato**: Gustavo Henrique Pereira Silva
- **WhatsApp**: (61) 98335-0225
- **Email**: gustavo@jupa2025.com.br

## 📄 Licença

Este projeto é propriedade do JUPA 2025 - Sínodo Bandeirante, Brasília.

## 🤝 Contribuição

Para contribuir com o projeto:
1. Faça um fork do repositório
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Abra um Pull Request

---

**JUPA 2025** - Jogos da União Presbiteriana de Adolescentes  
Sínodo Bandeirante • Brasília • 2025