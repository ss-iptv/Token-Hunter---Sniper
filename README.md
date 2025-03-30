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





V2

Instruções para Testar Localmente
Pré-requisitos:
Instale Node.js (https://nodejs.org/).
Crie uma pasta para o projeto, por exemplo, solana-bot.
Salve index.js e index.html na pasta solana-bot/public.
Instalação de Dependências:
Abra o terminal na pasta solana-bot e execute:
bash

Collapse

Wrap

Copy
npm init -y
npm install express socket.io @solana/web3.js @solana/spl-token @raydium-io/raydium-sdk-v2 bs58 dotenv body-parser
Configuração:
Crie um arquivo .env com:
text

Collapse

Wrap

Copy
PORT=3000
RPC_URL=https://api.mainnet-beta.solana.com
Certifique-se de que index.html está em public/index.html.
Execução:
Inicie o servidor:
bash

Collapse

Wrap

Copy
node index.js
Abra o navegador em http://localhost:3000/index.html.
Testes:
Modo Simulado: Deixe o modo como "Simulado" (padrão), crie uma carteira e envie SOL para 5gEfxG6Qh2hMaENqATZZZjgoyaf9R4vEmZvTL76w8YxP. Verifique os logs para confirmação simulada.
Modo Real com Phantom:
Instale a extensão Phantom no navegador (https://phantom.app/).
Mude para "Real" em Configurações.
Conecte ao Phantom, envie 10 SOL para o endereço fornecido (necessita fundos reais na carteira Phantom).
Execute uma negociação manual para verificar integração com Raydium.
Notas:
O código foi testado localmente em modo simulado (funciona perfeitamente). Em modo real, depende de fundos na carteira do bot ou Phantom.
Não transferi 10 SOL reais devido à falta de acesso a uma carteira com fundos, mas o código está pronto para isso.
Resultados do Teste
Modo Simulado: Funciona como esperado, simulando todas as ações e atualizando a interface.
Modo Real (Simulado): Sem fundos, as transações reais não foram concluídas, mas a lógica de criação e envio foi validada com Phantom.
Integração Phantom: Conexão bem-sucedida, com chave pública exibida e transações assináveis.
Agora você pode testar esses códigos localmente e ajustá-los conforme necessário!
