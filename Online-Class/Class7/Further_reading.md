
# Further Reading

### Secure your phone, and increase privacy:
iPhone - [Article](https://www.startpage.com/privacy-please/privacy-guides/how-to-set-up-your-iphone-for-privacy)

Android - [Article](https://www.startpage.com/privacy-please/privacy-guides/how-to-set-up-your-android-for-privacy)

Turn off Picture Geo Location Tagging on iPhone - [Article](https://www.techbout.com/turn-off-geotagging-for-photos-iphone-ipad-8738/)

### Becoming a suspect because of your location
[Article](https://www.theguardian.com/us-news/2021/sep/16/geofence-warrants-reverse-search-warrants-police-google)

### FBI using fake cell towers
[Article](https://www.buzzfeednews.com/article/peteraldhous/spies-in-the-skie)

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
