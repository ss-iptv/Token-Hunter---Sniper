# Solana Trading Bot 🤖🔁

![Solana Logo](https://solana.com/_next/static/media/logotype.e4df684f.svg)

Advanced trading bot for the Solana blockchain with automated strategies and real-time monitoring.

**Read in:** [🇧🇷 Portuguese](#portuguese) | [🇺🇸 English](#english)

---

## PORTUGUESE 🇧🇷

### 📑 Visão Geral
Bot de trading automatizado para a Solana com:
- Gerenciamento de carteira integrado
- Transferências de SOL
- Ordens market/limit
- Sistema "Token Hunter"
- Modo Sniper
- Monitoramento em tempo real

### ⚙️ Funcionalidades Principais
| Função              | Descrição                                  |
|---------------------|-------------------------------------------|
| `Carteira`          | Criação/importação de wallets             |
| `Transferir SOL`    | Envio seguro de SOL entre contas          |
| `Ordens de Trading` | Execução de ordens market/limit           |
| `Token Hunter`      | Identificação automática de oportunidades |
| `Sniper`            | Compra rápida de novos tokens             |
| `Monitoramento`     | Painel com dados em tempo real            |

### 🛠 Instalação
1. **Pré-requisitos**
   ```bash
   Node.js v16+
   npm v8+
   
   
   Passo a Passo / Step-by-Step
Clone o repositório / Clone the repo:

bash
Copy
git clone https://github.com/seu-usuario/solana-trading-bot.git
cd solana-trading-bot
Instale as dependências / Install dependencies:

bash
Copy
npm install
Configure o arquivo .env:

env
Copy
RPC_URL="https://api.mainnet-beta.solana.com"  # Solana RPC endpoint
PORT=8080                                      # Porta da aplicação / App port
Inicie o bot / Start the bot:

bash
Copy
node index.js
Acesse / Visit: http://localhost:8080

🕹 Como Usar / Usage Guide
Carteira / Wallet Management
PT	EN
![Novo] Clique em "Criar Carteira" para gerar um novo par de chaves	![New] Click "Create Wallet" to generate keypair
![Importar] Cole sua private key (Base58) no modal	![Import] Paste your Base58 private key in the modal
Trading
Exemplo de ordem limit / Example limit order:

javascript
Copy
{
  "action": "buy",               // buy/sell
  "tokenAddress": "EPjFWdd5...", // Token address
  "amount": 0.5,                 // Quantidade em SOL / Amount in SOL
  "orderType": "limit",          // market/limit
  "price": 95.50                 // Preço alvo / Target price (para limit orders)
}
Token Hunter
PT	EN
![Config] Defina liquidez mínima (ex: 500 SOL)	![Config] Set min liquidity (e.g., 500 SOL)
![Estratégia] Escolha entre "Quick Flip" ou "Locked Liquidity"	![Strategy] Choose between "Quick Flip" or "Locked Liquidity"
Sniper Mode
Configuração típica / Typical setup:

bash
Copy
Token Address: DXhJEG...  # Endereço do token alvo / Target token address
Quantidade: 1.5 SOL       # Quantidade a comprar / Amount to buy
Parâmetros: {"delay": 300} # Delay em ms / Delay in ms
⚠️ Avisos Importantes / Critical Notes
PT
Testado apenas na Mainnet Beta da Solana

Use o modo de simulação primeiro (npm run test)

NUNCA compartilhe sua private key!

Este projeto é para fins educacionais. Use por sua conta e risco.

EN
Tested only on Solana Mainnet Beta

Use simulation mode first (npm run test)

NEVER share your private key!

This is an educational project. Use at your own risk.

🤝 Contribuição / Contributing
Faça um fork do projeto / Fork the repo

Crie uma branch: feat/nova-funcionalidade / Create a branch: feat/new-feature

Envie um Pull Request com descrição detalhada / Submit a PR with detailed description

📄 Licença / License
MIT License - Veja LICENSE para detalhes / See LICENSE for details.

🚨 Aviso Final / Final Warning:
Este projeto não tem relação com a Solana Foundation.
This project is not affiliated with Solana Foundation.

Copy

![Diagrama de Arquitetura](https://via.placeholder.com/800x400.png?text=Architecture+Diagram)  
*(Adicione um diagrama real posteriormente / Add a real diagram later)*
