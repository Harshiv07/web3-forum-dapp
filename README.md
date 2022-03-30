# Basic Web3 Forum

This project demonstrates a basic web3 forum that requires signing of the accounts in order to submit to the forum, anyone can view the previous comments, and is deployed on [polygon testnet](https://mumbai.polygonscan.com/) with `0xFB0AAe92c2f2efbFA71D7BD0Cad5B742B5707427` 

Try running some of the following tasks:

```shell
npx hardhat accounts
npx hardhat compile
npx hardhat clean
npx hardhat test
npx hardhat node
node scripts/sample-script.js
npx hardhat help
```

## Setup

1. git clone
2. npm i
3. npx hardhat compile
4. npx hardhat test
5. npx hardhat node
6. create an .env file with `PRIVATE_KEY=<your-private-key>` (Private key of metamask acc)
7. npx hardhat run --network localhost scripts/deploy-and-seed.js
8. npm run dev

In order to run on localhost:8545,
1. Change provider to localhost `const provider = providers.getDefaultProvider(
  "http://localhost:8545"
);
` in pages/index.ts
2. Change addressOrName to your contract address after step 7 from setup`addressOrName: "deployed-contract-address",` in hooks/useCommentsContract.ts
