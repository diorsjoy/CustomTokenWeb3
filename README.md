# CustomTokenWeb3

This repository contains JavaScript code for interacting with a custom Ethereum token deployed on the Sepolia test network using Infura.

## Usage

Run the JavaScript script to interact with the custom Ethereum token:

```bash
node index.js
```

## Demo Screenshots

Put demo screenshots or GIFs showcasing the usage of your code here.

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
