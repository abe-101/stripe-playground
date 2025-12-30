# Stripe Payment Method Tester

A simple browser-based tool for testing Stripe SetupIntents and saving payment methods. Useful when you need to test Stripe integrations without access to your application's frontend.

## Live Demo

[https://abe-101.github.io/stripe-playground](https://abe-101.github.io/stripe-playground)

## Features

- **Stripe Connect support** - Test with connected accounts
- **Standard mode** - Test with regular Stripe accounts
- **Payment Element** - Uses Stripe's modern Payment Element UI
- **Copy to clipboard** - Easily copy the resulting Payment Method ID

## Usage

1. Enter your Stripe **Publishable Key** (`pk_test_...`)
2. If using Stripe Connect, enter the **Connected Account ID** (`acct_...`)
3. Paste your **SetupIntent Client Secret** (`seti_..._secret_...`)
4. Click **Initialize** to load the Payment Element
5. Enter test card details (e.g., `4242 4242 4242 4242`)
6. Click **Save Payment Method** to confirm the SetupIntent
7. Copy the resulting Payment Method ID for use in your backend

## Test Cards

| Card Number | Description |
|-------------|-------------|
| 4242 4242 4242 4242 | Succeeds |
| 4000 0000 0000 3220 | Requires 3D Secure |
| 4000 0000 0000 9995 | Declined |

Use any future expiry date and any 3-digit CVC.

## Local Development

Just open `index.html` in your browser. No build step required.

## License

MIT
