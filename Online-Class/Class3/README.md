# Securing E-Mail Communications

### Brief History of E-Mail
E-mail is one of the first forms of communication on the internet (the first email was sent in 1971).  E-mail is very insecure, and not much has been changed in the technology to fix that.  When you type an e-mail, and click Send, the following steps occur:

- Your words are stored (as text) in your Sent folder (either on your e-mail server, or your local computer)
- A copy is handed to your e-mail server (as text), who then does a query of the DNS server to know where to send it
- A connection is made to the recipient's e-mail server, and a copy (as text) is sent to that server
- Where it is stored (as text) until your intended recipient connects, and retrieves it (as text)

### Why the Emphasis on "as text"
As an e-mail travels from server to server, and person to person, that message can be captured, copied, read, forwarded, etc.  A good rule of thumb, when writing an e-mail message, is to not write anything that you wouldn't want read by the entire world.  Most of us don't share secrets over e-mail, and so, aren't worried about it.  But, sometimes we forget that the message is readable by the world, and when a spouse sends a quick e-mail, or SMS/TXT (which is also transmitted as text, needing your Health Insurance member number, your Social Security number, etc.), and you respond without thinking about it (since it is your spouse), you may have just opened yourself up to any number of evils: Identity Theft, Banking Theft, etc. - depending on the information shared (but also, definately captured, and stored forever by the NSA [surveilance computers](https://en.wikipedia.org/wiki/PRISM_(surveillance_program))).

### Solutions?
Even though e-mail is nearly a 50 year old technology, and there are many other forms of communication, we continue to use e-mail for many things.  There are tools which allow for encrypting messages, prior to sending, and this requires extra software for the sender, the receiver, and a sharing of public keys between each sender and receiver combination.  Another solution, is to switch e-mail providers to a service which stores all of your e-mail in an encrypted state (incoming new e-mail, sent-mail, archived email - all of it).  The only person who can read your e-mail is you.  One such service is called [Protonmail.com](https://protonmail.com) . Protonmail is an e-mail server that has encryption built-in (no extra software needed, and they generate your encryption keys for you).  If you want to send an encrypted message to someone who doesn't have your public key, and isn't using an account on the Protonmail servers, Protonmail will allow you to set a password for that message, and the reciever will get an e-mail with a link.  That link will open a page on their web browser, prompt for the password you set, and unencrypt the message (on the website, leaving the message encrypted on the Protonmail server).  The reciever can even reply to you via this web page (making their message encrypted as well).

Even if you don't replace your primary e-mail with the Protonmail account, at least you have the option when you would like to send securely encrypted and stored messages.

### Phishing
While we are on the subject of e-mail, we should discuss "phishing".  Phishing, is much like "going fishing".  Someone who wants information only you have (like, bank account login credentials, or shopping sites which might already your credit card saved), will send you an e-mail, crafted to trick you into clicking on a link, and typing in the information they are looking for.

Here is a rather convincing Phishing e-mail I received recently:

![Phishing_email](phish.png)

This e-mail appears, at first, to be a receipt from Amazon for an order I supposedly placed.  The Phisher, wanted me to believe that my account with Amazon had been compromised, and click on the "View or manage order" button.  If I hadn't noticed that this wasn't an e-mail from Amazon, I might have clicked that button (or in fishing terms, taken the bait).  Most likely, the button would have opened up a web page on my browser, and that page would've looked like a login page for Amazon. If I had typed in my login information, it wouldn't have logged me into Amazon, but most likely given an error, and I would have tried over and over, giving up, and trying a different way (as I would've been frantic to cancel the $2600.00 order).  In the background, that "fake" Amazon login page was sending my username and password to the person/group who sent the Phishing e-mail, and they would login to Amazon as me, change my password (so that I couldn't log in and make any changes), and then hope that a credit card was attached, and then proceed to order whatever they pleased, having the items shipped to them, instead of me, and leaving me with the bill (and frustration of fighting the charges, getting a new credit card, etc.).

Now, it is possible, the Phisher wouldn't have had it quite that easy.  I'm sure you've been prompted, and even required, for websites like banks, Amazon, etc., to add an extra step of security to your account.  This is called 2FA (2-Factor Authentication).  The idea behind 2FA authentication is that if someone obtains your username and password, they need a 3rd item (which should be in your physical possession).  Most websites suggest that you provide your cell phone number, and they will send you a Text/SMS message (a code), and since you are always in physical possession of your phone, that will insure your account will not get hacked.  Unfortunately, accounts continue to get hacked.  The issue?  Phone companies are easily manipulated, by persistent smooth talkers, who convince them to transfer your phone number to their cell phone - so that, they will receive the 2FA TXT/SMS code, and login as you.

### How did I know it was a Phishing E-Mail?
Before I discuss a better 2FA option, and leave behind this sample Phishing e-mail, you might be asking if I clicked the button.  I did not.  After my initial panic, I calmly looked at the e-mail message sitting in my inbox, and noticed it was missing the Amazon logo, and the blue text wasn't clickable.  But, the biggest give away was the sender's e-mail address.  Notice that it was sent from an account with an @gmail.com address.  Companies send e-mails, not from personal accounts, but from company e-mail accounts.  There are some real tricky ways to make the sender e-mail address look like it is from the company e-mail domain, but it is very hard to do (currently), thus rare.

The best rule of thumb: if you receive an e-mail you weren't expecting (and/or it looks even slightly suspicious), don't click any links in the message.  If you receive an order receipt/confirmation like this one, instead of clicking the button: open your browser, login to your Amazon account, and look to see if that order shows in your account.  If the order is there, then the order is real, and either your spouse ordered something with your account, or your account was hacked.  If the order isn't there, just delete the e-mail, and be thankful you didn't fall for their tricks.  For more things to look out for in Phishing e-mails, see the "Additional Reading" section below.

### Better 2FA
If SMS messages can be intercepted (didn't mention that before, but they can - and remember, they are sent "as text" : except iPhone to iPhone, those are encrypted, but Apple holds the encryption key), what is a person to use for 2FA?  If your bank, or other website, only support SMS/TeXT for 2FA, I would suggest applying pressure (and providing supporting documentation) to the website to encourage them to offer other 2FA options.

E-mail is often an option that is offered, and I believe that protects you from the easily persuaded cell phone employee, but again, e-mail is sent "as text".

The most secure option is some "Authenticator" application, which is installed on your phone (see "Additional Reading" for suggestions).  The "Authenticator" applications allow you to add multiple accounts (one for each website), and they provide you with ever changing numerical codes (displayed in the application), which you type into the website.  These are rather technical in nature to explain, so I will refer you to "Additional Reading" section if you would like to read more about how they work.  The short of it though: use them if they are offered by your bank, or website - and if they don't offer that option yet, apply pressure to persuade them to offer it soon.

<<-- [Previous Class](../Class2/README.md) -- [Next Class](../Class4/README.md) -->>

Additional Reading:
[Further_Reading](Further_reading.md)
