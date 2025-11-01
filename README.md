3. ERC-1155 (Multi-Token – Mixed Fungible and Non-Fungible)
Core Functions
-balanceOf(address account, uint256 id)→ Returns how many tokens of a given ID an address owns.
-balanceOfBatch(address accounts, uint256 ids)→ Returns multiple token balances in a single call.
-setApprovalForAll(address operator, bool approved)→ Grants or revokes permission for an operator to manage all your tokens.
-isApprovedForAll(address account, address operator)→ Checks if an operator can manage all tokens of a specific account.
-safeTransferFrom(address from, address to, uint256 id, uint256 amount, bytes data)→ Safely transfers a specific amount of one token type.
-safeBatchTransferFrom(address from, address to, uint256 ids, uint256 amounts, bytes data)→ Safely transfers multiple token types in one transaction.
Internal Functions
_mint(address to, uint256 id, uint256 amount, bytes data) → Creates new tokens of a specific type.
_mintBatch(address to, uint256[] ids, uint256 amounts, bytes data)→ Creates multiple token types at once.
_burn(address from, uint256 id, uint256 amount)→ Destroys a specified amount of one token type.
_burnBatch(address from, uint256[] ids, uint256 amounts) → Destroys multiple token types in a single transaction.
