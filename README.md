# BUG when using pnp with esm loader and playwright

The bug happens with node `v14.17.0`.
Testing it on node `v16` and above the bug doesn't happen.

## How to reporduce the bug.

1. Clone this repo.
1. Run `yarn && yarn test`
1. Watch playwright getting stuck.
1. In the file `.yarnrc.yml`, set `pnpEnableEsmLoader` to `false`.
1. Run `yarn && yarn test`. Now everything works.
