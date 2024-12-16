# Project Description
## Manual Installation

clone the repo:
```bash
git clone https://github.com/ikezuby2012/riseIn-bc
```
Install the dependencies:

```bash
yarn install
```
## Project Files
### Airdrop.ts
The airdrop.ts script allows you to airdrop a specified amount of lamports to the wallet address stored in the dev-wallet.json file.

Run Command on Console
```bash ts-node ./airdrop.ts
Success! Check out your TX here:
        https://explorer.solana.com/tx/5k4wiycZ7GaF3pLcWzm6WRDpdax1tnqpmtkSu5qgZfENTNXGpR3QWXXYKgJPfDVGns86UQmzMS8GPVQMaBHGUwL1?cluster=devnet
```

### transfer.ts
The airdrop.ts script allows you to transfer a specified amount of lamports to the public address specified in the program.

Run Command on Console
```bash yarn transfer
yarn run v1.22.22
$ ts-node ./transfer.ts
Success! Check out your TX here:
        https://explorer.solana.com/tx/4QJjdgSGgpKd8BNmPKyjFNFpg5Rcy7KHF8oLmS9nR5S5cXTA3LNiGqdka469Ukff3MnAXK3aLTeeaGRBkYNqv225?cluster=devnet
Done in 24.41s.
```
### programs/wba_prereq.ts
This file contains the Program IDL

### enroll.ts
This script interacts with the Solana blockchain using the specified IDL (wba_prereq). It performs a transaction calling the complete method of the program, sending a GitHub username as input, and signing the transaction with the wallet stored in dev-wallet.json. The script generates and logs a transaction hash that can be used to verify the transaction on the Solana blockchain explorer

```bash yarn enroll
$ ts-node ./enroll.ts
Success! Check out your TX here:
  https://explorer.solana.com/tx/5RXEsNwAo62HeWCyYc28bZ1b3uY7ZJNPndqHt85zXCXSsceVh1sf28FT2H38s9zxVUZHSqzNuzfhbp2JnRMAc5iX?cluster=devnet
Done in 15.02s.
```