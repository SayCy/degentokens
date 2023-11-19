# DegenToken

DegenToken is a simple ERC-20 token on the Ethereum blockchain with additional functionality to add items, view item prices and quantities, and buy items using the token.

## Smart Contract Details

- **Name**: DegenToken (Symbol: DGN)
- **Standard**: ERC-20
- **Version**: Solidity ^0.8.18

## Functionality

1. **Add Item**
   - `addItem(string memory itemName, uint256 price, uint256 quantity)`: Allows the owner to add an item with a specified price and quantity.

2. **Get Item Information**
   - `getItemPrice(string memory itemName)`: Retrieves the price of a specific item.
   - `getItemQuantity(string memory itemName)`: Retrieves the available quantity of a specific item.

3. **Buy Item**
   - `buyItem(string memory itemName, uint256 quantity) payable`: Allows users to buy a specified quantity of an item by paying with Degen tokens. The item's quantity is reduced, and the buyer's tokens are burned.

4. **Mint Tokens**
   - `mint(address to, uint256 amount)`: Allows the owner to mint new Degen tokens and send them to a specified address.

5. **Burn Tokens**
   - `burn(uint256 amount)`: Allows users to burn their own Degen tokens.

6. **Token Transfer**
   - `transfer(address to, uint256 amount)`: Overrides the ERC-20 `transfer` function to provide custom logic.
