# Elhadaba 🤖

A simple chatbot made with just HTML, CSS and JavaScript. No frameworks, no server, nothing to install.

## How to run it

1. Download `elhadaba.html`
2. Double click it (it opens in your browser)
3. Start chatting!

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
