# 📑 **Documentação do Projeto: Node Farm**

---

## 🛠 **Visão Geral do Projeto**

**Node Farm** é um projeto desenvolvido em **Node.js** sem o uso de frameworks externos, focado no aprendizado dos conceitos fundamentais do Node, como leitura e escrita de arquivos, criação de servidor HTTP, roteamento básico e manipulação de templates.

---

## 📂 **Estrutura do Projeto**

```
node-farm/
├── data
│   ├── data.json                 # Dados dos produtos em formato JSON
│   └── template-product.html     # Template HTML para exibir cada produto
├── dev-data
│   └── data.json                 # Dados de desenvolvimento
├── templates
│   ├── overview.html             # Template para a página principal
│   ├── product.html              # Template para a página de produtos individuais
│   └── card.html                 # Template para cada cartão de produto
├── src
│   ├── index.js                  # Servidor principal em Node.js
│   └── replaceTemplate.js        # Função para substituir dados no template
├── .env                          # Variáveis de ambiente
└── README.md                     # Documentação do projeto
```

---

## 🚀 **Funcionalidades**

- **Servidor HTTP:** Criação de um servidor local para servir arquivos HTML e dados dinâmicos.
- **Roteamento Simples:**
  - `/` ou `/overview`: Exibe uma visão geral dos produtos.
  - `/product?id=0`: Exibe os detalhes do produto específico.
  - `/api`: Retorna os dados do produto em formato JSON.
  - **404:** Para rotas desconhecidas.
- **Renderização Dinâmica de Templates:** Substituição dinâmica dos placeholders nos templates HTML.
- **Tratamento de Erros:** Exibição de uma página de erro para rotas inexistentes.

---

## 🔗 **Rotas da Aplicação**

| Método | Rota               | Descrição                                  |
| ------ | ------------------ | ------------------------------------------ |
| GET    | `/` ou `/overview` | Exibe a página inicial com os produtos.    |
| GET    | `/product?id=0`    | Exibe detalhes do produto selecionado.     |
| GET    | `/api`             | Retorna o JSON de todos os produtos.       |
| GET    | `*`                | Exibe página de erro para rotas inválidas. |

---

## 💻 **Passo a Passo para Executar o Projeto**

1. **Clone o Repositório:**

```bash
git clone https://github.com/seu-usuario/node-farm.git
cd node-farm
```

2. **Inicie o Servidor:**

```bash
node src/index.js
```

3. **Acesse a Aplicação:**

- Abra o navegador e vá para: `http://localhost:8000`

