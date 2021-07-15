From https://dev.to/dabit3/the-complete-guide-to-full-stack-ethereum-development-3j13

## notes

Found a bug in the instructions. `hardhat.config.js` needs this line at the top:

`require("@nomiclabs/hardhat-waffle");`

Or you get issues with `deploy.js` on this line:

`const Greeter = await hre.ethers.getContractFactory("Greeter");`

because `hre.ethers` is undefined
