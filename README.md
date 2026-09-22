# Elhadaba 🤖

A simple chatbot made with just HTML, CSS and JavaScript. No frameworks, no server, nothing to install.

## How to run it

1. Download `elhadaba.html` (on GitHub open the file, then click the download button - do NOT copy the text off the page)
2. Make sure the name still ends in `.html` and not `.html.txt`
3. Double click it, it opens in your browser
4. Type a message and press Enter or click Send

## If nothing happens when you send

- Check the file name really ends in `.html`
- Open it in Chrome, Firefox, Edge or Safari, not in a text editor or Notepad
- Viewing it on the GitHub website only shows the code, it does not run it
- Press F12 and look at the Console tab, any red error there tells you what is wrong

## How it works

- Everything is in one file: `elhadaba.html`
- The bot has a "brain" which is just a list of keywords and answers
- When you send a message it looks for a keyword it knows and replies
- If you share an idea (like "I think..." or "what if...") it praises it first
- It can also do simple maths like `12 * 4`

## Adding more knowledge

Open the file and find the `brain` list. Add a new line like this:

```js
{ keys: ["pizza"], answer: "Pizza is the best food ever 🍕" },
```

That's it, now Elhadaba knows about pizza.
