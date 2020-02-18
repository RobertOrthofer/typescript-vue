# typescript-test

## Project setup

Project setup:

    vue create typescript-vue

Options:
  - manual setup
  - Selected Features:
    - typescript
    - Linter/Formatter
  - class style component syntax: NO
  - babel along typescript: NO
  - linter: ESLint + standard config
  - lint on save
  - config in package.

Changes from initial config: [07f465b](https://github.com/RobertOrthofer/typescript-vue/commit/07f465b2c2421df6f7fd98229f76225b6f5f52c8)


## Observed behaviour
The computed property `foo` in [`HelloWorld.vue`](https://github.com/RobertOrthofer/typescript-vue/blob/07f465b/src/components/HelloWorld.vue#L41-L44) has an incorrect return type.

When running [`npm run typecheck`](https://github.com/RobertOrthofer/typescript-vue/blob/07f465b/package.json#L9) no errors are shown.

## Expected behaviour
tsc should report an error similar to the one vetur detects
![vetur-error](./Screenshot%202020-02-18%20at%2012.07.27.png)
