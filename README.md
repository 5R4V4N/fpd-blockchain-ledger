<div align="center">

# fpd-blockchain

fake product identification on the blockchain

[![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)](https://soliditylang.org)
[![Truffle](https://img.shields.io/badge/Truffle-5E464D?style=flat-square&logo=truffle&logoColor=white)](https://trufflesuite.com)
[![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)](https://ethereum.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

</div>

---

a decentralized app (DApp) that lets users verify product authenticity on-chain. scan a product's QR code with your camera, the app queries the smart contract, and you instantly know if it's real or counterfeit — no central database, no middleman.

---

## stack

**blockchain**
- **truffle suite** — smart contract compilation, testing, and deployment
- **solidity** — smart contracts in `contracts/`
- **@truffle/hdwallet-provider** — wallet signing and network connectivity

**frontend**
- **html + css + js** — plain UI with Bootstrap (compiled from SASS in `src/scss/`)
- **lite-server** — lightweight local server for the static frontend
- **html5-qrcode** — camera-based QR code scanning for product verification

---

## setup

```bash
git clone https://github.com/5R4V4N/fpd-blockchain.git
cd fpd-blockchain
npm install
```

you'll also need truffle installed globally:

```bash
npm install -g truffle
```

for local blockchain testing, install [Ganache](https://trufflesuite.com/ganache) and have a workspace running before you migrate.

---

## running it

start the frontend:

```bash
npm run dev
```

then open `http://localhost:3000`.

---

## smart contract commands

compile contracts into JSON artifacts (`build/`):

```bash
truffle compile
```

deploy to your active Ganache workspace or a testnet:

```bash
truffle migrate
```

force redeploy if contracts already exist:

```bash
truffle migrate --reset
```

run unit tests in `test/`:

```bash
truffle test
```

---

<div align="center">
made by <a href="https://github.com/5R4V4N">@5R4V4N</a>
</div>
