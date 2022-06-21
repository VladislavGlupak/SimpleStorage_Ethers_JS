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

4. `yarn add ethers` - install `Ethers`
5. `yarn add fs-extra`
6. `node deploy.js` - deploy
