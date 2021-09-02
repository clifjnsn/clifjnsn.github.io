# DNS (Domain Name Services)
DNS is the service which takes the human readable website/server URL's and translates them into the the numeric addresses which computers understand.

For example, this class is hosted on [GitHub](https://github.com), which is the same as 140.82.113.3 (IP address).

When you type github.com into your browser, or click on a link to this class from your email, a DNS server looks up the computer address (IP Address), and provides it back to your computer, then your browser contacts the server at the IP address, and requests to have the information it is storing, and your browser displays it for you.

What would happen if this database, which holds the list of translations from human readable words to IP addresses were hacked, or changed to have bad information?  Or, what happens if you miss-type the human readable words?  In the case of mistyping, you might simply get an error, like "Site not found".  But, you could be re-directed to a server you didn't intend to visit.  This server could have malware, pornography, or try to trick you into entering your username/password for the location you intended to visit, so that someone could steal your account.

There are several DNS services that provide very good DNS lookup databases, and even provide some corrections for your miss-typed words, and a list of "bad" websites which can be blocked for you: so that you are not exposed to the malware, pornography, or potentially have your account/password stolen.

The company that I feel provides the best set of services, and does this for free for families, is [OpenDNS](https://opendns.com) .

Their "Family Shield" product doesn't require an account, you simply update the DNS settings on your devices and/or modem/router, and you get the benefit of this safer database.

For detailed instructions on how to do this, visit the [FamilyShield](https://www.opendns.com/setupguide/#familyshield) Website.
