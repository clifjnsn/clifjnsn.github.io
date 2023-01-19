
# Further Reading

Monero Website [website](https://www.getmonero.org/)

Book: Mastering Monero by Serhack [website](https://masteringmonero.com/)

Deep Dive Learning of Monero [website] (https://learnmonero.co)

Bitcoin/Blockchain Explorer [transaction](https://www.blockchain.com/explorer/addresses/btc/bc1qk94cx7l8g36pztah6lxv6r4sdsuy8g6c2rplwt)

This transaction shows that someone sent over $40,000 to 2 other wallets.  Following the wallet addresses, someone could track down who
the money was ultimately sent to (what wallet address), and findout how much money was in that wallet (as the balance is public information), and
do more research to findout where that person lives, or target them with Phishing email, in an attempt to gain access to that wallet, and transfer
the funds to their wallet).

<!-- Read the Formbutton docs at formspree.io/formbutton/docs. See more examples at codepen.io/formspree -->
<script src="https://formspree.io/js/formbutton-v1.min.js" defer></script>
<script>
  /* paste this line in verbatim */
  window.formbutton=window.formbutton||function(){(formbutton.q=formbutton.q||[]).push(arguments)};
  /* customize formbutton below*/     
  formbutton("create", {
    action: "https://formspree.io/f/xleazppa",
    title: "How can we help?",
    fields: [
      { 
        type: "email", 
        label: "Email:", 
        name: "email",
        required: true,
        placeholder: "your@email.com"
      },
      {
        type: "textarea",
        label: "Message:",
        name: "message",
        placeholder: "Do you have a question I might be able to answer?",
      },
      { type: "submit" }      
    ],
    styles: {
      title: {
        backgroundColor: "gray"
      },
      button: {
        backgroundColor: "gray"
      }
    }
  });
</script>
