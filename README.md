# dss-proxy-actions
Initial version of the proxy functions to be used via ds-proxy. These functions are based on dss-cdp-manager as CDP registry.

https://github.com/makerdao/dss-proxy-actions

`open`: creates a registry in CdpManager

`give`: transfer the ownership of a CDP in the internal registry of CdpManager

`lockETH`: deposits ETH in adapter and executes `frob` increasing locked collateral

`lockGem`: deposits ERC20 Collateral in adapter and executes `frob` increasing locked collateral

`freeETH`: executes `frob` decreasing locked collateral and withdraws ETH from adapter

`freeGem`: executes `frob` decreasing locked collateral and withdraws ERC20 Collateral from adapter

`draw`: executes `frob` increasing debt and exits token (minting it) from DAI adapter

`wipe`: joins token to the DAI adapter (burns it) and executes `frob` for decreasing debt

`lockETHAndDraw`: combines `lockETH` and `draw`

`openLockETHAndDraw`: combines `open`, `lockETH` and `draw`

`lockGemAndDraw`: combines `lockGem` and `draw`

`openLockGemAndDraw`: combines `open`, `lockGem` and `draw`

`wipeAndFreeETH`: combines `wipe` and `freeETH`

`wipeAndFreeGem`: combines `wipe` and `freeGem`
