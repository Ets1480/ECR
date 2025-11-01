
1. ERC-20 (Fungible Token – Like Coins)
Core Functions
-totalSupply → Returns the total number of tokens in existence.
-balanceOf(address account)→ Shows how many tokens a specific address owns.
-transfer(address to, uint256 amount)→ Sends tokens from your account to another address.
-approve(address spender, uint256 amount)→ Authorizes another address to spend your tokens.
-allowance(address owner, address spender) → Checks how many tokens a spender is allowed to use from an owner’s account.
-transferFrom(address from, address to, uint256 amount)→ Moves tokens from one address to another using the allowance mechanism.
Internal Functions
_mint(address account, uint256 amount)→ Creates new tokens and adds them to the specified account.
_burn(address account, uint256 amount)→ Destroys tokens from the specified account.
2. ERC-721 (Non-Fungible Token – Unique Items)
Core Functions
-balanceOf(address owner)→ Returns how many NFTs a specific address owns.
-ownerOf(uint256 tokenId)→ Returns the current owner of a specific NFT.
-approve(address to, uint256 tokenId)→ Grants permission for another address to transfer a specific NFT.
-getApproved(uint256 tokenId)→ Returns the address approved to transfer a specific NFT.
-setApprovalForAll(address operator, bool approved)→ Allows or revokes another address’s permission to manage all your NFTs.
-isApprovedForAll(address owner, address operator)→ Checks if an operator can manage all NFTs of an owner.
-transferFrom(address from, address to, uint256 tokenId)→ Transfers ownership of an NFT from one address to another.
-safeTransferFrom(address from, address to, uint256 tokenId)→ Safely transfers an NFT, ensuring the recipient can handle it.
Internal Functions
_mint(address to, uint256 tokenId)→ Creates a new NFT and assigns it to the specified address.
_burn(uint256 tokenId)→ Destroys a specific NFT.
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
