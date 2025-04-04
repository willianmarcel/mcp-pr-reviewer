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
- Conta no GitHub
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
python main.py
```

O serviço irá:
1. Conectar-se à API do GitHub
2. Monitorar PRs especificados
3. Realizar análise automática
4. Gerar documentação no Notion

## 🛠️ Arquitetura

O projeto é estruturado em três componentes principais:

- `main.py`: Ponto de entrada da aplicação
- `pr_analyzer.py`: Core da análise de PRs
- `github_integration.py`: Integração com a API do GitHub

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
