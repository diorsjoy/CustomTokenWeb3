# CustomTokenWeb3

This repository contains JavaScript code for interacting with a custom Ethereum token deployed on the Sepolia test network using Infura.

## Usage

Run the JavaScript script to interact with the custom Ethereum token:

```bash
node index.js
```

## Demo Screenshots
<img width="835" alt="image" src="https://github.com/diorsjoy/CustomTokenWeb3/assets/113359068/1e7d88e3-8212-46e0-99ae-c6580f53775f">

<img width="426" alt="image" src="https://github.com/diorsjoy/CustomTokenWeb3/assets/113359068/ef943f56-fa82-45a8-9b47-67efbef67382">

<img width="814" alt="image" src="https://github.com/diorsjoy/CustomTokenWeb3/assets/113359068/4bbc5cca-38e1-4b1c-aebb-41168c3cc9b7">

## Examples

getBalance function to get a current balance of the account

```javascript

const customTokenContract = new web3.eth.Contract(contractABI, contractAddress);

async function getBalance(address) {
    try {
        const balance = await customTokenContract.methods.balanceOf(accountAddress).call();
        console.log(`Balance of ${accountAddress}:`, balance);
    } catch (error) {
        console.error('Error retrieving balance:', error.message || error);
    }
}

```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

Special thanks to [OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts) for inspiration.

```
