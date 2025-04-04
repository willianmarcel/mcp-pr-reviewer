# PR Reviewer 🔍

Um assistente inteligente para análise de Pull Requests que integra GitHub com Notion para documentação automatizada de revisões.

## 🌟 Características

- Análise automática de Pull Requests do GitHub
- Integração com Notion para documentação estruturada
- Interface MCP (Model-Controller-Provider) para processamento eficiente
- Suporte a análise detalhada de mudanças de código
- Geração automática de documentação no Notion

## 🚀 Começando

### Pré-requisitos

- Python 3.8 ou superior
- Conta no GitHub com token de acesso
- Conta no Notion com permissões de API
- Tokens de acesso configurados

### Instalação

1. Clone o repositório:
```bash
git clone [seu-repositorio]
cd pr_reviewer
```

2. Crie e ative um ambiente virtual:
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# ou
.venv\Scripts\activate  # Windows
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

4. Configure as variáveis de ambiente:
Crie um arquivo `.env` com as seguintes variáveis:
```env
NOTION_API_KEY=seu_token_do_notion
NOTION_PAGE_ID=id_da_pagina_notion
GITHUB_TOKEN=seu_token_do_github
```

## 💻 Uso

Para iniciar o analisador de PRs:

```bash
python pr_analyzer.py
```

O serviço irá:
1. Inicializar o servidor MCP para análise de PRs
2. Estabelecer conexão com a API do GitHub
3. Configurar a integração com o Notion
4. Aguardar solicitações de análise de PRs
5. Gerar documentação automaticamente no Notion

## 🛠️ Arquitetura

O projeto é estruturado em dois componentes principais:

- `pr_analyzer.py`: Core da aplicação que gerencia o servidor MCP e coordena as análises
- `github_integration.py`: Módulo responsável pela integração com a API do GitHub

### Componentes

#### PR Analyzer
- Inicializa o servidor FastMCP
- Gerencia a integração com o Notion
- Registra ferramentas para análise de PRs
- Processa as solicitações de análise

#### GitHub Integration
- Gerencia a comunicação com a API do GitHub
- Recupera informações de Pull Requests
- Processa mudanças de código

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👥 Contribuição

Contribuições são bem-vindas! Por favor, sinta-se à vontade para submeter PRs.

1. Faça um Fork do projeto
2. Crie sua Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📞 Suporte

Se você encontrar algum problema ou tiver sugestões, por favor abra uma issue no repositório.

---

Desenvolvido com ❤️ pela equipe Avanade
