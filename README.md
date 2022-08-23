# Fractal - Treasury Module

## Architecture

The Treasury Module utilizes the MVD accessControl and moduleBase to deal with permissions. 


### TreasuryModule.sol

The Treasury Contract contains the methods needed to deposit and withdraw ERC20, ERC721, and ERC1155, Ether. It is important that the contract inherits from the Module base contract in order to handle authorized permissions.


### TreasuryModuleFactory.sol

The Treasury Factory Contract contains the methods needed to deploy a proxy that is pointed to an implementation on chain. It is important this contract inherits from the ModuleBaseFactory interface so that is compatible with the metaFactory contract in the MVD.

## Local Setup & Testing

Clone the repository:
```shell
git clone ...
```

Lookup the recommended Node version to use in the .nvmrc file and install and use the correct version:
```shell
nvm install 
nvm use
```

Install necessary dependencies:
```shell
npm install
```

Add `.env` values replacing the private key and provider values for desired networks
```shell
cp .env.example .env
```

Compile contracts to create typechain files:
```shell
npm run compile
```

Run the tests
```shell
npm run test
```

## Deploy Contract to <network>
```shell
npx hardhat deploy --network <network>
```

## Local Hardhat deployment

To deploy the base Fractal contracts open a terminal and first run:
```shell
npx hardhat node
```

This will deploy the following contracts and log the addresses they were deployed to:
 - TreasuryModuleFactory
 - Treasury Implementation

