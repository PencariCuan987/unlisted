npm install
nvm use 20

curl -L https://foundry.paradigm.xyz | bash
source /home/gitpod/.bashrc
foundryup

wget -qO - 'https://proget.makedeb.org/debian-feeds/prebuilt-mpr.pub' | gpg --dearmor | sudo tee /usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg 1> /dev/null
echo "deb [arch=all,$(dpkg --print-architecture) signed-by=/usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg] https://proget.makedeb.org prebuilt-mpr $(lsb_release -cs)" | sudo tee /etc/apt/sources.list.d/prebuilt-mpr.list
sudo apt update && sudo apt install just
just install
cp .env.example .env
Search File .Env - Open File .env - Edit & Isi .env di Bawah :
- File ada di pojok kiri tinggal scroll
- Use New Wallet

PRIVATE_KEY_1='Your Private Key ETH'

OP_ALCHEMY_API_KEY='PASTE API KEY From ALCHEMY'
BASE_ALCHEMY_API_KEY='PASTE API KEY From ALCHEMY'
OP_BLOCKSCOUT_API_KEY='PASTE API KEY From BLOCKSCOUT'
BASE_BLOCKSCOUT_API_KEY='PASTE API KEY From BLOCKSCOUT'

➡️ ADD API KEY - Alchemy :
➖ Link : https://dashboard.alchemy.com/apps
➖ Create New APP (OP Sepolia) - Copy & Paste Code API KEY di .env
➖ Create New APP (Base Sepolia) - Copy & Paste Code API KEY di .env
➖ Claim Faucet Base, OP Sepolia : https://warpcast.com/horsefacts.eth/0x518ad874
➖️ Search RPC On Chainlist.org
➖️ Send Faucet To Your New Wallet
➖ Done 
➖ After Received, Move Next Step 

➡️ ADD API KEY Blockscout : 
➖ Link : https://optimism-sepolia.blockscout.com/account/api-key
➖ Add API KEY (Your Name) Copy & Paste Code API KEY di .env
➖ Open Link : https://base-sepolia.blockscout.com/account/api-key
➖ Add API KEY (Your Name) Copy & Paste Code API KEY di .env
➖ Click ︙On Top Right > Closed Save All

➖ Back To Terminal Paste :
just do-it




📖 Source Docs : https://docs.polymerlabs.org/docs/quickstart/start/
