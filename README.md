# Algorand NFT Mint

Créer un NFT Algorand

### Dependencies:
- Algorand SDK 
- PureStake API
- dotenv

### Fichiers:

#### 1.`generate_algo_account.js` creates a fundable account on Algorand

- Créer un compte 
- Un mnemnonic, une clé privée
- Génère l'adresse du compte



#### 2. `generate_nft.js` creates a single Algorand NFT/ASA via Javascript SDK / PureStake

- Génère le NFT / ASA



#### 3. `generate_algo_account.js` asset creation template


### How to use the files: 
- clone repo => run `npm install`
- Avoir un environement de dev (j'utilise VSC perso, en complément Docker peut être utilisé).
1. Aller sur purestake.com pour avoir son compte et sa clé API. On utilise l'API PureStake API pour intéragir avec la blockchain Algorand. Penser à faire aussi son compte Pinata pour upload les images (ou autre, mais pour avoir des URL).
2. Créer un fichier .env
3. Faire son compte Algo `node generate_algo_account.js`
4. Ajouter sa clé API key to `generate_nft.js `
5. Ajouter son mnemonic `generate_nft.js` 
6. Mettre les données relatifs au NFT via l'URL
7. Minter le NFT `node generate_nft.js`

### Successful Ouput:
- Si tout va bien, le terminal affichera les données du NFT et de la transaction
`
PPSWJDI6HOBJGSGV3L5GXUXMCLNIX4P53JNUGJEJBA5LEXLXNS67MIQ2IE
Transaction : G6T2EYO6AKFXQQR2NQ2UDMFNYSRB4YUNWW7SUKFMJZ4XQKOVOS3A
Transaction confirmed in round 22305958
`
- Allez sur Algoexplorer pour voir la transaction (un exemple ici: https://testnet.algoexplorer.io/tx/4X3KPNIDJHXA2P7MVIKZN22QFFPJVGPGMMLOT3ZEOSF5NDM56RKQ).