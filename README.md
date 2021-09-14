# Rapyd Checkout Toolkit Demo

Quickly integrate Rapyd Checkout Toolkit into your online shopping cart

[![thumbnail of video link for youtube video showing rapyd checkout toolkit video](https://files.readme.io/a4897c1-Youtube_Thumbnail_-_Rapyd_Bytles_-_Checkout_Toolkit2x.png)](https://youtu.be/3a788d8NFCc)


This repository contains a simple example demonstrating how to add Rapyd's Checkout Toolkit to an eCommerce website. Checkout Toolkit lets you embed an iframe directly into your shopping cart payment acceptance fields. This ensures your customers are never redirected away from your website during the checkout process.

Visit Rapyd's documentation where you can see more code samples and watch a demo video: https://docs.rapyd.net/build-with-rapyd/docs/checkout-toolkit

To use this example:

1. Clone this repository.
2. Create a checkout page using the API: https://docs.rapyd.net/build-with-rapyd/reference/checkout-page-object#create-checkout-page
3. Copy the checkout page id from the API response (for example, "checkout_123456789123456789123456789")
4. Open the checkout.html file and find the code below. Paste the checkout id in the "id" field:

```javascript
let checkout = new RapydCheckoutToolkit({
    pay_button_text: "Pay Now",
    pay_button_color: "#4BB4D2",
    id: "checkout_", // your checkout page id goes here
    style: {
        submit: {
            base: {
                color: "white"
            }
        }
    }
});
```
Checkout toolkit integration documentation:

https://docs.rapyd.net/build-with-rapyd/docs/checkout-toolkit
