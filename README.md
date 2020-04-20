[![Version](https://img.shields.io/npm/v/@adobe/asset-compute-eslint-config.svg)](https://npmjs.org/package/@adobe/asset-compute-eslint-config)

# asset-compute-eslint-config

Central ESlint configuration for Adobe Asset Compute

This is set up as a shareable config in the adobe scope as described [here](https://eslint.org/docs/developer-guide/shareable-configs)

## Adding Central ESlint Config to Asset Compute Repositories

1. Install the Asset Compute eslint config:

`npm install @adobe/asset-compute-eslint-config --save-dev`

2. Create or edit the `.eslintrc.js` file inside the action and add `@adobe/asset-compute-eslint-config` as an extension:

```node
module.exports = {
    "extends": "@adobe/asset-compute-eslint-config",
};
```

3. Add any other specific rules needed for the action to the config file.
4. For any [Mocha](https://mochajs.org/) tests, add the following below the copyright notice: `/* eslint-env mocha */`
5. Run `npx eslint ./`


### Contributing
Contributions are welcomed! Read the [Contributing Guide](./.github/CONTRIBUTING.md) for more information.

### Licensing
This project is licensed under the Apache V2 License. See [LICENSE](LICENSE) for more information.
