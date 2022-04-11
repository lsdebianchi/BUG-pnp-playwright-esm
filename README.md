# BUG when using pnp with esm loder and playwright

## How to reporduce the bug.

Clone this repo.
Run:
`yarn && yarn test`
Watch the test runner getting stuck.
In the file `.yarnrc.yml`, set `pnpEnableEsmLoader` to `false`.

Run:
`yarn && yarn test`

Now everything works.
