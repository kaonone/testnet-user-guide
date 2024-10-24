
# Kaon Testnet User Documentation

**Kaon Core Team**  
*October 3, 2024*

This document introduces the Kaon testnet and guides users through how to access Kaon, its key features, and its applications. Our aim is to equip developers, builders, and partners with the knowledge to effectively explore, test, and innovate within the Kaon ecosystem.

## 1. Accessing the Testnet

Welcome to the Kaon blockchain ecosystem. For an in-depth analysis of the network, please proceed to our testnet explorer: [Kaon Testnet Explorer](https://explorer.testnet.kaon.one).

This explorer, while based on the classic Ethereum-type model, has been adapted to efficiently handle our UTXO chain data stream. The transformation process is transparent and publicly accessible, featuring the following key adaptations:

1. Full integration of Recursive Length Prefix (RLP) encoding.
2. Implementation of 1e-18 as the native denomination.
3. Conversion of UTXO transactions into Ethereum-compatible format.

The primary interface of the explorer features an "Add Kaon Testnet" button located at the bottom of the screen. Selecting this button will integrate the Kaon Testnet into your MetaMask application. Please note that this functionality is currently limited to the browser-based MetaMask wallet.

Manual configuration of the Kaon Testnet is possible for any Ethereum-compatible wallet using the following network parameters:

- **Network designation**: Kaon Testnet
- **RPC endpoint**: https://testnet.kaon.one
- **Chain identifier**: 11989
- **Native currency symbol**: KAON
- **Block explorer URL**: https://explorer.testnet.kaon.one

Upon successful configuration, you will have established a functional account on the Kaon network. However, users will notice that they currently have 0 KAON tokens.

## 2. Testnet Tokens

To acquire complimentary tokens for testing purposes, navigate to the Kaon Testnet Faucet at [http://faucet.testnet.kaon.one](http://faucet.testnet.kaon.one). Select the “Faucet” option to initiate the token distribution process.

On the faucet interface, input your MetaMask wallet address and specify the desired token quantity. The interface also displays your Kaon UTXO format address, which corresponds to your Ethereum format address.

Upon completion of the request, a confirmation notification will be displayed. Token distribution typically occurs within a 60-second timeframe, barring any network congestion or technical issues.

## 3. Generate a New Token

Upon successful acquisition of testnet tokens, you can now deploy a new ERC20-compliant token using the simplified token generation interface available at [https://tokengen.testnet.kaon.one](https://tokengen.testnet.kaon.one).

Once your MetaMask is connected, you may customize and deploy any desired token configuration within the parameters provided by the platform.

## 4. Interacting with Uniswap V2 on Kaon Testnet

After deploying a token, you may explore additional functionalities within the Kaon ecosystem. For instance, you can interact with our deployed instance of Uniswap V2, accessible at [https://uniswap.testnet.kaon.one//swap](https://uniswap.testnet.kaon.one//swap). This allows users to test token swapping and liquidity provisioning within the Kaon testnet environment.

To engage with the Uniswap V2 instance on the Kaon testnet, follow these procedural steps:

1. **Acquire Wrapped Ether (WETH)**:
   - The exchange rate is fixed at 1 WETH = 1 KAON.
   - Transfer your KAON tokens to the WETH contract address: `0x11e465D214d00A37A11C67796b7fC4DD15dbCCB9`
   - You will receive an equivalent amount of WETH in return.
   
2. **Token Integration**:
   - Add the token you previously created to your wallet interface.

3. **Liquidity Provision**:
   - After acquiring WETH, navigate to the Uniswap interface.
   - Create a trading pair using your custom token and WETH.
   - Establish a liquidity pool for this pair.

4. **Trading Initiation**:
   - With the liquidity pool established, you may commence trading activities.

This process enables you to simulate and test various DeFi operations within the controlled environment of the Kaon testnet.

## 5. Building on Kaon

For advanced contract deployment and interaction, the [Remix Ethereum IDE](https://remix.ethereum.org) offers a versatile platform. This integrated development environment can be connected to the Kaon testnet through various methods:

- MetaMask integration
- TrustWallet connection
- Direct network connection

Upon successful connection, you can proceed to deploy and test your smart contracts within the Kaon testnet environment. It is noteworthy that the network fully supports EVM Shanghai, providing access to the latest Ethereum Virtual Machine features and optimizations.
