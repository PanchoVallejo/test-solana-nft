# General guide for uploading nfts
Full guide: https://www.quicknode.com/guides/web3-sdks/how-to-deploy-an-nft-collection-on-solana-using-sugar-candy-machine
## Steps to upload a test nft on Windows 

1. Install Sugar & solana on cmd

2. Set up api test net on solana 

``solana config set --url https://api.devnet.solana.com``

3. Generate a new wallet

``solana-keygen new --outfile .test-keys/test-wallet.json``

4. Configure solana to use the generated keys 

``solana config set --keypair test-keys/test-wallet.json``

5. Check wallet balance & add some test balance 

``solana balance``

``solana airdrop 2``

6. Upload the NFTs! 

``sugar upload``

``sugar deploy``

``sugar verify``

7. Mount Candi machine UI & install yarn dependencies

``git clone https://github.com/metaplex-foundation/candy-machine-ui ./candy-machine-ui/``

## Steps to upload a real nft on Windows 

1. Set up api main net on solana
``solana config set --url https://api.mainnet-beta.solana.com``
