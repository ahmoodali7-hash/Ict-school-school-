# Digital business card

A one-page contact card for Mahmoud Abdelfattah Ali, Building Inspector at the
Department of Housing, Government of Sharjah. Scanning `qr-code.png` opens it.

## What's in this folder

- `index.html` - the card page
- `logo.png` - the Department of Housing logo shown at the top
- `mahmoud-abdelfattah-ali.vcf` - the contact file the Save to Contacts button opens
- `qr-code.png` - the QR code to print, it opens the card page

## Every row is a link

| Row | What happens when you tap it |
| --- | --- |
| Direct line | Calls +971 56 151 6663 |
| Email | Opens a new email to mahmoud.mobark@dh.sharjah.ae |
| Department | Calls +971 6 504 4444 |
| Website | Opens www.dh.sharjah.ae |
| Save to Contacts | Adds "Mahmoud Abdelfattah Ali" with mobile 056 151 6663 to the phone |

On iPhone the Save button opens the "Create New Contact" screen. On Android it
downloads the contact, tap it and choose Contacts to save it.

## Putting it online (GitHub Pages)

1. Repo **Settings** > **General** > scroll to the bottom > **Change visibility** > **Public**
   (free GitHub accounts can only use Pages on public repos)
2. **Settings** > **Pages**
3. Under **Build and deployment** pick **Deploy from a branch**
4. Choose the branch that has this `card` folder and the `/ (root)` folder, then **Save**

After a minute or two the card is live at:

https://ahmoodali7-hash.github.io/Ict-school-school-/card/

That is the address inside `qr-code.png`. If the card ever moves somewhere
else, the QR code has to be made again with the new address.

## Changing the details

Phone numbers and email appear in two places, so change both:

- the text and the `href="tel:..."` / `href="mailto:..."` links in `index.html`
- the `TEL` and `EMAIL` lines in `mahmoud-abdelfattah-ali.vcf`
