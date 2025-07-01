# Github config and workflows

In this folder there is configuration for dependabot and ci workflows
that check the library more deeply than the default configurations.

This folder can be or was merged using a --allow-unrelated-histories merge
strategy from <https://github.com/byfnoel/rust-infra/> which provides a
reasonably sensible base for writing your own ci on. By using this strategy,
the history of the CI repo is included in your repo, and future updates to
the CI can be merged later.

To perform this merge run:

```shell
git remote add ci https://github.com/byfnoel/rust-infra.git
git fetch ci
git merge --allow-unrelated-histories ci/main
```
