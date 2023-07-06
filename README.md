# app-tokens
Whitelisted token assets and list

The JSON schema for the tokens includes: chainId, name, address, decimals, symbol, logoURI. Required!

#

Adding or Updating a token

1- Fork the repository

2- Add the new token at the end of the token array in piteas-tokenlist.json

  Please make sure that the new token follows this schema.

    {
        "chainId": 369, // Should always be 369
        "address": "token_address on Pulsechain",
        "name": "token_name",
        "symbol": "token_symbol",
        "decimals": <token_decimals>,
        "logoURI": "token_icon_uri",
    }

  #Example token query
  - "chainId": 369,
  - "address": "0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07",
  - "name": "USD Coin from Ethereum",
  - "symbol": "USDC",
  - "decimals": 6,
  - "logoURI": "https://raw.githubusercontent.com/piteasio/app-tokens/main/token-logo/0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07.png"

3- Commit the changes and raise a PR to our repo's dev branch.

#

Disclaimer
After raising a PR, please allow us some time to verify the PR. We do not follow any particular order in reviewing token additions and updations.
