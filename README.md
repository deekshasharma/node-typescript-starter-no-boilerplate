
## Where is the `tsconfig.json` file?
- Default `tsconfig.json` is used by ts-node. When in doubt, ts-node --show-config will log the configuration being used, and ts-node -vv will log node and typescript versions.
Since `ts-node` is installed locally, it should be used with `npx` prefix.
```shell
npx ts-node --show-config
```

## How to start the app using our own `tsconfig.json` file?

Add the following in your `package.json` `start` script
```shell
    "start": "ts-node --project tsconfig.json src/index.ts",
```

## Open questions | things to be done
- How will the output directory be generated with the JS files?
- Add Husky pre-commit hook for linting
- Add prettify


