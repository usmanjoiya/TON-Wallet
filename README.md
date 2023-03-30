# TON-Wallet
Integration for any website with TON using wallets compatible with TON NETWORK

In this code, you first define two buttons with IDs connect-wallet-button and connect-keeper-button. 
You then add event listeners to these buttons that connect to TON Wallet and TON Keeper respectively.

When the connect-wallet-button is clicked, the code creates a TON client using the TONClient.create() method and sets up the client with your app key. 
It then creates a signer using your public key and gets the deployment address for the signer. 
Finally, it creates a new TON wallet using the client, signer, and address, and stores it in the window.wallet variable.

When the connect-keeper-button is clicked, the code uses the TonWeb.requestPermissions() method to request permission to use the TON Keeper signer. 
If the user grants permission, the code displays an alert indicating that the user has been connected to TON Keeper.

Note that you will need to replace YOUR_APP_KEY and YOUR_PUBLIC_KEY with your own app key and public key respectively. 
You will also need to make sure that the TON SDK is loaded on your website before this code is executed.
