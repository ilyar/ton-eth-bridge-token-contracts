# FT

Setup `giver` https://everscale-org.github.io/intro

```shell
yarn
yarn se-reset
wget https://raw.githubusercontent.com/EverscaleGuild/locklift-sample/main/locklift.config.js
yarn compile
```

## Create account

Create manual via `Ever Wallet` account `<wc:account>` and `topup`
```shell
npx everdev contract topup \
  --network se \
  --value 100000000000 \
  --address <wc:account>
```

or

```shell
yarn local-deploy-account --key_number 0
```

## Deploy FT token

```shell
yarn local-deploy-root \
  --root_owner <wc:account> \
  --name 'Be Test Coin' \
  --symbol BTC \
  --decimals 8 \
  --initial_supply_to <wc:account> \
  --initial_supply 21000000 \ 
  --disable_mint false \
  --disable_burn_by_root false \
  --pause_burn false
```
