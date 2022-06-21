Please, install:

1. `corepack enable`
2. `yarn add solc@0.8.7-fixed`
3. Compile
   `yarn solcjs --bin --abi --include-path node_modules/ --base-path . -o . SimpleStorage.sol`
   or

add to `package.json`

```
{
	"dependencies": {
		"solc": "0.8.7-fixed"
	},
	"scripts": {
		"compile": "yarn solcjs --bin --abi --include-path node_modules/ --base-path . -o . SimpleStorage.sol"
	}
}
```

and run `yarn compile`
