# Avax_Proof_M3
# NToken Smart Contract

This smart contract defines a simple token named "BLING" with the symbol "BG". It allows the owner to mint new tokens, burn existing tokens, and transfer tokens between addresses.

## Key Components

### 1. Owner
- **Owner:** The address that deployed the contract and has special permissions, such as minting new tokens.

### 2. Token Details
- **Token Name:** BLING
- **Token Symbol:** BG
- **Total Supply:** The total number of tokens that have been minted.

### 3. Balances
- **Mapping:** Keeps track of the token balance of each address.

## Functions

### 1. `mint`
- **Purpose:** Mint new tokens.
- **Restrictions:** Only the owner can mint tokens.
- **Logic:** Increases the total supply and the balance of the specified address by the given amount.

### 2. `burn`
- **Purpose:** Burn existing tokens.
- **Logic:** Decreases the total supply and the balance of the specified address by the given amount if the address has sufficient tokens.

### 3. `transfer`
- **Purpose:** Transfer tokens from one address to another.
- **Logic:** Transfers the specified amount of tokens from the sender's address to the recipient's address if the sender has sufficient tokens.

## Modifiers

### 1. `onlyOwner`
- **Purpose:** Restrict certain functions to be executed only by the owner.
- **Logic:** Checks if the caller is the owner. If not, it throws an error.

## License

This contract is licensed under the MIT License.
