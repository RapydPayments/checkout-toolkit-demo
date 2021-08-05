# Rapyd Checkout Toolkit Demo
Rapyd checkout toolkit integration demo

This repository contains a simple example that shows the implementation of Rapyd's checkout toolkit into an eCommerce website.

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

~  
Isaac Benitez
@Rapyd