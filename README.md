> [!IMPORTANT]
> **Projeto arquivado (11/10/2026).** O BacenTools agora é um site 100% estático, sem esta API: o navegador busca os dados direto da BrasilAPI e do Banco Central.
> Código atual, testes e documentação: **[vieiraes/bacentools](https://github.com/vieiraes/bacentools)** · site: **https://bacentools.web.app**

# BacenTools

![Logo BacenTools](https://img.shields.io/badge/BacenTools-Ferramentas%20para%20Meios%20de%20Pagamento-blue)

BacenTools é uma coleção de ferramentas voltadas para desenvolvedores e POs (Product Owners) que trabalham com meios de pagamento e integrações com o sistema financeiro brasileiro.

🔗 **Acesse agora:** [bacentools.web.app](https://bacentools.web.app)

## 📌 Visão Geral

Este projeto visa simplificar o trabalho com integrações de pagamento e regulações do BACEN (Banco Central do Brasil), oferecendo ferramentas úteis para validação, consulta e visualização de informações relacionadas ao sistema financeiro nacional.

![BacenTools Screenshot](https://via.placeholder.com/800x400?text=BacenTools+Screenshot)

## 🚀 Funcionalidades

- **Consulta de Bancos**: Busque informações sobre instituições financeiras por ISPB, código COMPE ou nome
- **Cotações e Taxas**: Consulte cotações atualizadas de moedas e indicadores financeiros
- **Ferramentas PIX**: Validação de chaves, geração e decodificação de QR codes
- **Decoder JWT**: Ferramenta para decodificar e analisar tokens JWT usados em integrações financeiras

> ⚙️ **Nota para POs**: Novas funcionalidades estão sendo implementadas constantemente. Se precisar de uma ferramenta específica, por favor crie uma issue detalhando a necessidade.

## 🔧 Tecnologias Utilizadas

- **Frontend**: HTML5, CSS3, JavaScript, Alpine.js, Bootstrap 5
- **Backend**: Node.js, NestJS, TypeScript
- **Implantação**: Fly.io (Backend), Firebase Hosting (Frontend)

## 🏁 Começando

### Acesso Online

Acesse diretamente pelo navegador: [bacentools.web.app](https://bacentools.web.app)

### Instalação Local

#### Pré-requisitos

- Node.js (versão 16 ou superior)
- npm ou yarn

#### Instalação

1. Clone o repositório
   ```bash
   git clone https://github.com/seu-usuario/bacentools.git
   cd bacentools
   ```

2. Instale as dependências
   ```bash
   npm install
   ```

3. Execute o projeto em modo de desenvolvimento
   ```bash
   npm run start:dev
   ```

4. Acesse o projeto em http://localhost:3000

## 🧪 Testes

Execute os testes com o comando:
```bash
npm test
```

## 📱 API

A API BacenTools está disponível em:
- **Desenvolvimento**: http://localhost:3344/api
- **Produção**: https://bacentools-api.fly.dev/api

### Endpoints principais:

- `/api/banks` - Lista todas as instituições financeiras
- `/api/banks/ispb/{ispb}` - Busca banco por ISPB
- `/api/banks/code/{code}` - Busca banco por código COMPE
- `/api/banks/search?name={query}` - Busca bancos por nome

> 📘 **Nota para desenvolvedores**: Documentação completa da API disponível em `/api/docs` (Swagger).

# BacenTools API

API de ferramentas relacionadas ao sistema financeiro brasileiro.

## Descrição

BacenTools API é um backend NestJS que oferece endpoints para consulta de informações do sistema financeiro brasileiro, como bancos, cotações e participantes do PIX.

## Tecnologias

- NestJS
- TypeScript
- Axios para chamadas externas
- Fly.io para deployment

## Endpoints

### Bancos

- `GET /api/banks` - Lista todos os bancos
- `GET /api/banks/ispb/:ispb` - Busca banco por ISPB
- `GET /api/banks/code/:code` - Busca banco por código COMPE
- `GET /api/banks/search?name=:name` - Busca bancos por nome

## Executando o projeto

### Requisitos
- Node.js (versão 16 ou superior)
- npm ou yarn

### Instalação

```bash
# Instalar dependências
npm install

# Iniciar em desenvolvimento
npm run start:dev

# Compilar para produção
npm run build

# Iniciar em produção
npm run start:prod
```

## 📋 Para Product Owners

### Valor de Negócio

BacenTools foi desenvolvido pensando em acelerar o trabalho de equipes de desenvolvimento e POs que lidam com integrações financeiras. Algumas aplicações práticas:

- **Validação rápida**: Verificar se uma chave PIX está no formato correto durante demonstrações ou testes
- **Troubleshooting**: Decodificar tokens JWT em tempo real durante a investigação de problemas
- **Consulta eficiente**: Obter informações precisas sobre instituições financeiras sem precisar navegar pelo site do BACEN
- **Decisões informadas**: Acompanhar cotações e taxas para tomar decisões estratégicas sobre produtos financeiros

### Roadmap

O BacenTools é um projeto em constante evolução. Algumas funcionalidades planejadas:

1. **Validação de boletos**: Ferramenta para validar a linha digitável e o código de barras de boletos bancários
2. **Simulador de cálculos financeiros**: Cálculos de juros, parcelamentos e CET (Custo Efetivo Total)
3. **Dashboard de estatísticas**: Visualização gráfica de indicadores financeiros
4. **Agenda BC**: Calendário de eventos e prazos importantes do BACEN

> 💡 **Sugestões são bem-vindas!** Se você tem uma ideia para uma nova ferramenta que seria útil no seu dia a dia com meios de pagamento, abra uma issue ou entre em contato.

### Feedback dos Usuários

Estamos comprometidos em melhorar constantemente o BacenTools. Seu feedback é fundamental para isso. Por favor, compartilhe suas experiências e sugestões através das issues do GitHub ou pelo formulário de contato em nossa página "Sobre".

## 📄 Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE.md para detalhes.

## 🤝 Contribuindo

Contribuições são bem-vindas! Confira CONTRIBUTING.md para guidelines sobre como contribuir com este projeto.

## ✉️ Contato

Para sugestões, dúvidas ou problemas, abra uma issue ou entre em contato através do email [contato@vieiraes.com].

---

<div align="center">
  <p>Desenvolvido com ❤️ para a comunidade de desenvolvimento de meios de pagamento</p>
  <div>
    <i class="fas fa-university" style="color: #0d6efd;"></i>
    <i class="fas fa-exchange-alt" style="color: #6c757d;"></i>
    <i class="fas fa-code" style="color: #198754;"></i>
  </div>
</div>