mkdir ICO
cd ICO
mkdir hardhat-tutorial
cd hardhat-tutorial
npm init --yes
npm install --save-dev hardhat
npm install --save-dev @nomicfoundation/hardhat-toolbox
npx hardhat   选择 Create a Javascript Project
npm install @openzeppelin/contracts

创建 ICryptoDevs.sol
创建 CryptoDevToken.sol

npm install dotenv
添加 .env  里面的两个参数
QUICKNODE_HTTP_URL="add-quicknode-http-provider-url-here"

PRIVATE_KEY="add-the-private-key-here"

添加 scripts/deploy.js

修改 hardhat.config.js

npx hardhat compile

npx hardhat run scripts/deploy.js --network goerli

-------
前端
ICO 目录下
npx create-next-app@latest
cd my-app
npm run dev
npm install web3modal
npm i ethers@5
修改 Home.modules.css
修改 pages/index.js


在目录my-app 下面创建目录constants 在下面创建文件index.js
配置四个参数
export const NFT_CONTRACT_ABI = "abi-of-your-nft-contract";
export const NFT_CONTRACT_ADDRESS = "address-of-your-nft-contract";
export const TOKEN_CONTRACT_ABI = "abi-of-your-token-contract";
export const TOKEN_CONTRACT_ADDRESS = "address-of-your-token-contract";

运行 npm run dev