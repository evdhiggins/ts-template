# TS Project Template

A simple typescript project template with testing and linting (Eslint + Prettier + Jest).

## Setup guide

1. Clone the template

    The easiest way to get started with this template is to use [degit](https://github.com/Rich-Harris/degit):

    ```sh
    # Clone into current directory
    $ npx degit evdhiggins/ts-template

    # Clone into my-new-project
    $ npx degit evdhiggins/ts-template my-new-project
    ```

2. Install all dependencies (`npm install`)
3. Update `package.json` with details specific to your project
4. Make any desired alterations to the included configuration files -- make it your own!

## Remarks

-   The current configuration uses `ESM` modules. If this is for a node project using commonjs modules, remove the `type` parameter from `package.json` and change `compilerOptions.module` in `tsconfig.json` to `"CommonJS"`
-   There is a separate `tsconfig` file so that the test files are run and linted correctly but not included in the build output. If you want to include the test files build, the `tsconfig.build.json` file can be removed and the `build` command in `package.json` can be updated to point at the only remaining `tsconfig`
