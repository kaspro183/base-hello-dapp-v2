# Hello Base – Message Board dApp (sans terminal)

Un tableau de messages on-chain pour **Base Sepolia (testnet)**. Tu peux publier des messages (≤ 280 caractères) et les lister depuis l'UI web (HTML/JS + ethers via CDN).

## Structure
```
contracts/MessageBoard.sol   # Contrat Solidity
frontend/index.html          # dApp web
abi/MessageBoard.json        # ABI du contrat
```

## Déployer le contrat via Remix (sans terminal)
1. Ouvre https://remix.ethereum.org
2. Crée `MessageBoard.sol` et colle le contenu de `contracts/MessageBoard.sol`.
3. Compile avec `^0.8.20`.
4. Dans MetaMask, sélectionne **Base Sepolia** (Chain ID `84532`).
5. Dans Remix, choisis **Injected Provider - MetaMask** et **Deploy**.
6. Copie **l'adresse du contrat**.

## Utiliser l'interface
1. Ouvre `frontend/index.html` (Chrome + MetaMask).
2. Colle l'adresse du contrat et clique **Charger le contrat**.
3. Écris ton message et clique **Publier**.
4. Clique **Rafraîchir** pour voir les derniers messages.

## Pousser sur GitHub (sans terminal)
1. Crée un nouveau repo sur GitHub.
2. **Add file → Upload files** et glisse le contenu de ce projet (`contracts/`, `frontend/`, `abi/`, `README.md`, `.gitignore`).
3. Message de commit (ex: `feat: message board dapp`) → **Commit changes**.

## Licence
MIT
