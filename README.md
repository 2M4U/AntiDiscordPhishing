# The Infamous Copy-pasta Anti Phishing/Scam Announcement
<img src="https://i.imgur.com/iGQeSJs.png" /><img src="https://i.imgur.com/EnrHyIW.png">



# How to **ACTUALLY** prevent it 
###### *instead of this __DUMB COPY PASTA__ information which is useless*

I've noticed a copy-pasta announcement thats been in circulation throughout the platform of Discord, I wanted to inform you this copy-pasta is actually uninformative as 2FA does not prevent any form of Nitro Scam/Phishing Links due the nature of the way these scammers/links work, they are designed to steal your accounts token, and by doing so they have full control of your account including changing the email address/password and much more to do with which ever account is compromised, therefore rendering 2FA useless attempt to fight back against these phishing links, however there are much more secure and more efficient means of protecting your account simply by doing the following:

[1] Implementing a checker in a discord bot to scan for such scam links using this API:<br>
https://phish.sinking.yachts/docs

[2] Using this freeware that is open sourced on GitHub to protect against most Discord Token stealers/jackers/phishing sites.<br>
https://github.com/andro2157/DiscordTokenProtector

The reason on why they can grab the token is due to Discords inability to enforce protection against these types of things gaining accessing to what's known as `localStorage`, for example with the discord app for PC itself, the app is built in Electron and they use what's known as `"safeStorage()"` to encrypt/decrypt `localStorage`, it is encrypted until the [`science`](https://discord.com/api/v9/science) end point requests a heartbeat from the application (using websockets) at which point the app then decrypts the token and stores it in `localStorage`, making it vulnerable to phishing/jacking/stealing attempts.

Just thought I would inform you as I've seen this copy-pasta alot over the past few weeks and still see alot of people being phished by this illusion of 2FA potentially stopping scammers, which triggered me into researching as to how they are doing it, and what measures to take fully to stop 99.9% of their attempts.


### Science Endpoint Preview:
<img src= "https://i.imgur.com/DXLmL4I.png"/>
