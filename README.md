# Bitcoin Wallet Generator

This is a simple project that allows the creation of Bitcoin wallets. The generator creates a new Bitcoin wallet, which consists of a private key, a public key, a corresponding Bitcoin address, a mnemonic phrase for easy backup and recovery. The project aims to provide an easy way to generate wallets for educational or personal use.

## Features

- Generation of a random private key.
- Generation of the associated public key.
- Creation of a valid Bitcoin address from the public key.
- Generation of a mnemonic phrase (BIP-39) for wallet backup and recovery.
- Optionally support **BIP-32** for generating multiple addresses from a single seed.
- Export of the keys, address and mnemonic.

## Technologies

- **JavaScript** - For logic and key generation.
- **`bitcoinjs-lib`** - JavaScript library for working with Bitcoin and cryptography.
- **`bip39`** - JavaScript library for generating BIP-39 mnemonic phrases.
- **`bip32`** - JavaScript library for implementing BIP-32 hierarchical deterministic wallets.

## Installation

Follow the steps below to set up the project in your local environment:

1. Clone the repository:

    ```bash
    git clone https://github.com/Diogo-Amaral/btc-wallet.git
    ```

2. Navigate to the project directory:

    ```bash
    cd btc-wallet
    ```

3. Install the dependencies:

    ```bash
    npm install
    ```

## Usage

Once the environment is set up, you can generate a new Bitcoin wallet with the following command:

```bash
node ./src/createWallet.js
```

This command will generate a private key, a Bitcoin address and a mnemonic phrase, displaying them in the terminal. You can save this information for future use.

#### Sample output:
```shell
Private Key: 5JkxyZsmtS8wVjYqbhRdyBbRh7B76a4E2ptwqaChC4U1JwTChV3
Bitcoin Address: 1LfVzq7V65WcfpGH7FwZDNKn9gjT9gxvq7
Mnemonic Phrase: apple banana zebra whiskey tiger sunset cloud moon mango pizza guitar
```

## Security Notices

- **Never share your private key or mnemonic phrase**. If someone gains access to them, they can access and spend the bitcoins in your wallet.
- **Keep your information secure**. The project was created for educational purposes and should not be used in production without proper security review.

## References
- https://www.dio.me/