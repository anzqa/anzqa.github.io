<p><meta name="viewport" content="width=device-width, initial-scale=1.0"></p>  
    
# Keybase: Stellar Wallet - Payments Manual   
  
This manual describes different ways to make payments over Stellar network using Keybase application wallet.  
  
### Introduction  
   
It is assumed that you are already a keybase user, and have a stellar account linked to your keybase.  
  
If you are new to Keybase or Stellar, check the corresponding homepages:  
- [keybase.io](https://keybase.io)  
- [stellar.org](https://stellar.org)  

Keybase is in essence a key ring, where users can list their public keys. And send/receive encrypted messages. It has options to list your online identities (social media profiles, websites, cryptowallet addresses, useraccounts of online forums etc). and ascertain your ownership of those identities.   
  
For now, we will just focus on Keybase's use as a chat application with built-in wallet for payments.   
  
## Payment Options:   
- **Pay in lumens**. Lumen (XLM) is the native asset on Stellar network.   
- **Pay in lumens; but displayed as other currency.**   
- **Pay directly in other currencies**. USD, EUR, GBP...  
- **Pay other assets**. User defined tokens, stocks etc.   
  
## Payment Methods:  
Keybase app allows you to make payments in different ways.  
1. In-chat payments inside teams  
2. In-chat payment inside personal chats (one-to-one chat with any particular user).  
3. Send option inside personal chats  
4. Send option in user profile  
5. Send option in wallet  
  
These different options are for your convenience. Depending on where you are in the app, one of the options will be easier to access than the other. There is also certian differences between an 'in-chat payment' and a payment via 'send option'.   
  
### Method 1, 2: In-chat payments:   
This option is convenient for making quick payments while you are engaged in a chat. It works in team chats as well as personal chats.   
To make a payment, you just type the transaction as text message within the chat window and hit send.   
  
Text format for in-chat payment is `+<amount><asset>@<username>`   
Example1: to send 1 lumens to anz, you type: `+1XLM@anz` and hit enter.  
Doing so will open a pop-up window asking for confirmation. And the transaction is finalized only after confirmation.  
  
Example2: if you send `+1USD@anz`, anz will receive lumens worth 1USD (nearly 15XLM as per current exchange rate).  
  
![example2](https://anz.keybase.pub/kbcb/ui/inchat-1USD.jpg)  
  
It is important to note that: In this method, the recipient will only receive lumens.   
You can specify the amount to be sent in any valid asset code; but the result will still be the lumen-equivalent of that amount.   
If you are thinking: what if the recipient had a trustline set for USD?   
The answer is still: No! currently in-chat payments does not work with path-payment.   
> Trustline is a setting to be enabled inside the wallet so as to deal (receive) assets other than XLM.  
> You can read more on trustlines [here](https://medium.com/@mojoflower/stellar-trustlines-explained-3008532ded7f) and further [here](https://blog.litemint.com/stellar-trustlines-dont-trust-verify/)  
  
Also note: There is no option to add memo text in this method.   
> memo_text is a public short message you attach to a transaction, for  identification or reference.  
  
  
### Method 3: Send option inside personal chats:   
This option is convenient for making a precise payment while you are engaged in a personal chat. Depending on your app version, you might have a '$' sign icon or '+' sign icon right to the text field. Tapping either of this icon shows an option to 'send lumens'. Selecting this would open a page to make the desired transaction.   
   
Generic Send Option Screen   
  
![Send-Option_General](https://anz.keybase.pub/kbcb/ui/send-option.jpg)  
Enter the desired amount, and click send to finalize the payment in Lumens "Strictly purely lumen".   
  
**Sending lumen-equivalent of other currencies**  
Clicking the 'Change' option under XLM will show several options to display the amount in other currencies. Keep in mind: the recipient will still receive the payment in Lumens. It is displayed as other currency only for our convenience.   
  
**Sending other assets**  
If the recipient accepts assets other than XLM, you will see a blue banner notifying the same. Selecting 'Send other assets' will show the option to 'Pick an asset'. Which will further list all the assets trusted by the recipient.   
  
![banner](https://anz.keybase.pub/kbcb/ui/banner.jpg)  
  
:point_down:    
    
![pick-asset](https://anz.keybase.pub/kbcb/ui/pick-asset.jpg)  
  
Select the desired asset, enter the amount and click send. Equivalent XLM will be deducted from your account, and the recipient will receive the payment in the selected asset itself.   
  
If you have enabled trustlines in your wallet, you can also pick that asset to be deducted from your wallet instead of XLM, provided you have sufficient funds in form of that asset.   

Sending and Receiving assets other than XLM is through a process known as **path-payment**.  
Here the transaction is fullfilled making use of intermediate transactions steps.  
  
Example3: You are sending 0.06USD, but selected that payment to be made using your BTC balance  
  
![path-payment](https://anz.keybase.pub/kbcb/ui/path-pay.jpg)   
  
So it follows the path: BTC > XLM > USD  
Or with more intermediate exchanges, which ever is least costly.   
  
What happens behind the scene is somewhat like this:  
1. You (Sender) make a trade offer for BTC  
2. Someone buys that BTC from you for XLM  
3. Someone else buys that XLM for USD  
4. USD thus sold reach your recipient.   

### Method 4: Send option in user profile:  
You lookup someone using keybase search and open their profile. or whenever you are viewing the profile of a person, you can make payment to that person from the profile page itself. (without starting a chat or going to your wallet). This is done by clicking the more menu `[...]` beside [Follow] and [Chat] buttons on the recipient profile.   
This opens a page similar to what is exaplined above. And procedure for payments are same. 
  
### Method 5: Send option in Wallet:  

Navigate to send option on Keybase app wallet: Hamburger-menu > Wallet > `[Send]` button  
  
![menu](https://anz.keybase.pub/kbcb/ui/menu.jpg)   
  
:point_down:  
  
![send-button](https://anz.keybase.pub/kbcb/ui/send.jpg)   
  
:point_down:  
  
This shows options to 'Send to a Keybase user' or by directly 'to Stellar address'.   
  
![address-type](https://anz.keybase.pub/kbcb/ui/add-type.jpg)   
  
Then you can search for the desired Keybase user, or Enter the Stellar account number.   
There is also a QR code scanner to make entering the stellar address easy.  
  
![search,qr](https://anz.keybase.pub/kbcb/ui/search,qr.jpg)  
  
What follows is a familiar screen as described previously. And procedure for payments are same.  
  

### footnotes:  
The best way to learn is by practicing. Try above methods to send some XLM to your friends or people who help you on keybase teams.    
Sending to some external exchanges might require adding a memo as mandatory.. :warning: watch-out for it!  
  
Disclaimer: This description of the Keybase user interface is based on personal interpretations as on 31OCT2019.   
Do let me know of any mistakes or errors. And your valuable suggestions.  
  
:rocket: Thank you! 

-----  
Donations> GCZ2DBOKHAZPAJOGX73DM4LRQAHK6QG6HB3YRYMGSDWWL5GQTMLQCGVW 
