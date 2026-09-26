# 📦 Q-AI Chain SDK

The official JavaScript/TypeScript SDK for interacting with the **Q-AI Chain Protocol**.

## Installation

```bash
npm install qai-chain-sdk
```

## Quick Start

```javascript
import { 
  createWallet, 
  sendTransaction, 
  getTransactions, 
  getRiskScore, 
  QAIError 
} from 'qai-chain-sdk';

// Initialize a wallet
const wallet = createWallet();

// Get the risk score for a potential transaction
try {
  const score = await getRiskScore(wallet.address, "0xDestinationAddress");
  console.log("Risk Score:", score);
  
  if (score < 80) {
    // Send a transaction
    const tx = await sendTransaction(wallet, "0xDestinationAddress", "1.5");
    console.log("Transaction Sent:", tx.hash);
  } else {
    console.warn("Transaction flagged as high risk!");
  }
} catch (error) {
  if (error instanceof QAIError) {
    console.error("SDK Error:", error.message);
  }
}
```

## Available Exports

- `createWallet()`: Generates or recovers a Q-AI network wallet.
- `sendTransaction(wallet, to, amount)`: Sends a secure transaction via the FastAPI Gateway.
- `getTransactions(address)`: Retrieves transaction history.
- `getRiskScore(from, to)`: Queries the AI Engine for the real-time anomaly risk score.
- `QAIError`: Standardized error class for network and protocol exceptions.
