# Getting Your OpenAI API Key

Interview Helper does not come with an AI account. You bring your own OpenAI API
key, and you pay OpenAI directly for what you use. The key stays on your machine
(Windows Credential Manager) and is never shared with anyone, including the app's
author.

This takes about five minutes.

## 1. Create an OpenAI account

Go to <https://platform.openai.com/> and sign up or sign in. This is the OpenAI
**developer platform**, which is separate from ChatGPT. A ChatGPT Plus
subscription does not include API access, and API usage is billed on its own.

## 2. Add a payment method and some credit

API usage is pay-as-you-go, so you need a small balance before a key will work.

**Sign in first.** The billing pages are part of a web app that only loads when
you are already signed in to <https://platform.openai.com/>. If you open a
billing link in a fresh tab and the page looks blank or broken, sign in first,
then try again, or reach billing through the menu instead of a direct link.

To reach billing:

1. Sign in at <https://platform.openai.com/>.
2. Click the **gear / Settings** icon, then choose **Billing**. (The direct link
   is <https://platform.openai.com/settings/organization/billing/overview>, but
   only use it once you are signed in.)
3. Click **Add payment details** / **Add to balance**, enter your card, and add a
   starting amount. The minimum is usually about $5, which is plenty for many
   practice sessions.
4. OpenAI uses prepaid credit. **Auto recharge** is on by default during setup —
   turn it off if you do not want automatic top-ups.

If the billing page still will not load, OpenAI's own help article is a stable
fallback: **How can I set up prepaid billing?** at
<https://help.openai.com/en/articles/8264644-how-can-i-set-up-prepaid-billing>.
You can also add a card directly at
<https://platform.openai.com/account/billing/payment-methods>.

If a key returns an "insufficient quota" or billing error, it almost always means
this step is missing.

## 3. Create the API key

1. Go to <https://platform.openai.com/api-keys>.
2. Click **Create new secret key**.
3. Give it a name like `Interview Helper` and create it.
4. **Copy the key now.** OpenAI shows it only once. If you lose it, delete that
   key and create a new one.

A key looks like a long string beginning with `sk-`. Treat it like a password:
anyone who has it can spend your credit.

## 4. Add the key to Interview Helper

1. Open Interview Helper and go to **Settings**.
2. Paste the key into the OpenAI API key field and save.
3. Use **Test Mode** to confirm the key works with a short microphone test.

The app stores the key in **Windows Credential Manager** under your Windows
account. It is not written into any file in the app folder and is not part of the
program you downloaded.

## 5. (Recommended) Set a spending limit

To avoid surprises, set a monthly usage limit in the billing dashboard under
**Limits**. As a reference, about 30 minutes of live transcription costs roughly
$0.51, plus a few cents for coaching.

## A note on which AI providers are supported

Right now, Interview Helper works with **OpenAI only**.

The app was designed so that other providers, such as Anthropic (Claude), could
be added later, and you may see provider-related wording in Settings. **Anthropic
support is not built yet.** Only one provider can be active, and for this version
that provider is OpenAI. An Anthropic API key will not work today. If Anthropic
support is added in a future release, it will be noted in the release notes.

## Keeping your key safe

- Never paste your key into a chat, email, screenshot, or public post.
- Do not commit it to any code repository.
- If you think a key was exposed, delete it on the API keys page and create a new
  one. Deleting a key immediately stops it from working.
