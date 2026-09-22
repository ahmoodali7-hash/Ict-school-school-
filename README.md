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
- Keywords match whole words only, so "hi" does not match inside "think"
- Repeated letters get squashed, so "hiii" and "helloo" still work
- Plurals work too, so "loops" finds "loop"
- If you share an idea (like "I think..." or "what if...") it praises it first

## Maths it can do

It understands symbols and words, so all of these work:

- `12 * 4` and `10 plus 10`
- `50 minus 8`, `6 times 7`, `100 divided by 4`
- `20% of 50`
- `square root of 144`

## What it knows about

Coding (HTML, CSS, JavaScript, Python, Java, C++, SQL, Git, variables, loops,
arrays, functions, APIs), science (gravity, DNA, atoms, planets, the human
body, electricity), maths (pi, primes, areas, algebra), geography (capital
cities, rivers, mountains, continents), plus school and study tips, jokes,
football and small talk.

## Adding more knowledge

Open the file and find the `brain` list. Add a new line like this:

```js
{ keys: ["pizza"], answer: "Pizza is the best food ever 🍕" },
```

That's it, now Elhadaba knows about pizza.
