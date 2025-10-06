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
  - "logoURI": "https://raw.githubusercontent.com/vouchrun/app-tokens/main/token-logo/0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07.png"

3- Commit the changes and raise a PR to our repo's dev branch.

#

# Notice:
Please keep in mind that not every token can be listed, and it will need to be approved by the Piteas team. Here are some basic requirements:
- The token must have at least $15K in major liquidity (LPs with liquid tokens)
- Liquidity pools must be integrated with Piteas
- The token's logo and details must be provided


# Disclaimer
After raising a PR, please allow us some time to verify the PR. We do not follow any particular order in reviewing token additions and updations.
