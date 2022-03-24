# FT

setup giver https://everscale-org.github.io/intro

```shell
yarn
yarn se-reset
wget https://raw.githubusercontent.com/EverscaleGuild/locklift-sample/main/locklift.config.js
yarn compile
```

create manual via Ever Wallet account and topup
```shell
npx everdev contract topup -n se -a <account> -v 100000000000
```
or 
```shell
yarn deploy-account --key_number 0
```

**Deploy root**
```shell
yarn local-deploy-root --root_owner 0:751ef03bcfd3ed78a8563521f744da97f9f7fe370d032b434c2afb928d6890dc --name 'Be Test Coin' --symbol BTC --decimals 8 --initial_supply_to 0:751ef03bcfd3ed78a8563521f744da97f9f7fe370d032b434c2afb928d6890dc --initial_supply 21000000 --disable_mint false --disable_burn_by_root false --pause_burn false
```
