# ITreasuryModule









## Methods

### depositERC20Tokens

```solidity
function depositERC20Tokens(address[] tokenAddresses, address[] senders, uint256[] amounts) external nonpayable
```

Allows the owner to deposit ERC-20 tokens from multiple addresses



#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses | address[] | Array of token contract addresses |
| senders | address[] | Array of addresses that the ERC-20 token will be transferred from |
| amounts | uint256[] | Array of amounts of the ERC-20 token that will be transferred |

### depositERC721Tokens

```solidity
function depositERC721Tokens(address[] tokenAddresses, address[] senders, uint256[] tokenIds) external nonpayable
```

Allows the owner to deposit ERC-721 tokens from multiple addresses



#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses | address[] | Array of token contract addresses |
| senders | address[] | Array of addresses that the ERC-721 tokens will be transferred from |
| tokenIds | uint256[] | Array of amounts of the ERC-20 token that will be transferred  |

### initialize

```solidity
function initialize(address _accessControl) external nonpayable
```

Function for initializing the contract that can only be called once



#### Parameters

| Name | Type | Description |
|---|---|---|
| _accessControl | address | The address of the access control contract |

### withdrawERC20Tokens

```solidity
function withdrawERC20Tokens(address[] tokenAddresses, address[] recipients, uint256[] amounts) external nonpayable
```

Allows the owner to withdraw ERC-20 tokens from multiple addresses



#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses | address[] | Array of token contract addresses |
| recipients | address[] | Array of addresses that the ERC-20 token will be transferred to |
| amounts | uint256[] | Array of amounts of the ERC-20 token that will be transferred  |

### withdrawERC721Tokens

```solidity
function withdrawERC721Tokens(address[] tokenAddresses, address[] recipients, uint256[] tokenIds) external nonpayable
```

Allows the owner to withdraw ERC-721 tokens from multiple addresses



#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses | address[] | Array of token contract addresses |
| recipients | address[] | Array of addresses that the ERC-721 tokens will be transferred to |
| tokenIds | uint256[] | Array of amounts of the ERC-20 token that will be transferred  |

### withdrawEth

```solidity
function withdrawEth(address[] recipients, uint256[] amounts) external nonpayable
```

Allows the owner to withdraw ETH to multiple addresses



#### Parameters

| Name | Type | Description |
|---|---|---|
| recipients | address[] | Array of addresses that ETH will be withdrawn to |
| amounts | uint256[] | Array of amounts of ETH that will be withdrawnnn |



## Events

### ERC20TokensDeposited

```solidity
event ERC20TokensDeposited(address[] tokenAddresses, address[] senders, uint256[] amounts)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses  | address[] | undefined |
| senders  | address[] | undefined |
| amounts  | uint256[] | undefined |

### ERC20TokensWithdrawn

```solidity
event ERC20TokensWithdrawn(address[] tokenAddresses, address[] recipients, uint256[] amounts)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses  | address[] | undefined |
| recipients  | address[] | undefined |
| amounts  | uint256[] | undefined |

### ERC721TokensDeposited

```solidity
event ERC721TokensDeposited(address[] tokenAddresses, address[] senders, uint256[] tokenIds)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses  | address[] | undefined |
| senders  | address[] | undefined |
| tokenIds  | uint256[] | undefined |

### ERC721TokensWithdrawn

```solidity
event ERC721TokensWithdrawn(address[] tokenAddresses, address[] recipients, uint256[] tokenIds)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddresses  | address[] | undefined |
| recipients  | address[] | undefined |
| tokenIds  | uint256[] | undefined |

### EthDeposited

```solidity
event EthDeposited(address sender, uint256 amount)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| sender  | address | undefined |
| amount  | uint256 | undefined |

### EthWithdrawn

```solidity
event EthWithdrawn(address[] recipients, uint256[] amounts)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| recipients  | address[] | undefined |
| amounts  | uint256[] | undefined |



## Errors

### UnequalArrayLengths

```solidity
error UnequalArrayLengths()
```







