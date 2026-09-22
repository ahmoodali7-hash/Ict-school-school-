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

## The assignment steps

When you open it, Elhadaba runs through the task steps first:

1. It is a chatbot, and it is called Elhadaba
2. It says "Hi! I'm Elhadaba, your chatbot. What is your name?"
3. It stores your answer in the `userName` variable
4. It says "Nice to meet you!"
5. It asks "What is your favorite subject?"
6. It uses if/else to reply differently:
   - ICT gets "Great choice! I love technology too!"
   - Math gets "Awesome! I like solving problems!"
   - anything else gets "That sounds interesting!"

The if/else part is this:

```js
if (matches(subject, "ict")) {
  answer = "Great choice! I love technology too!";
} else if (matches(subject, "math")) {
  answer = "Awesome! I like solving problems!";
} else {
  answer = "That sounds interesting!";
}
```

After that the intro is finished and you can chat normally about anything
below. Because your name is stored, you can also ask it "what is my name".

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

## Countries and cities

There is a table of 67 countries and 50 cities, so you can ask things like:

- `capital of japan`
- `tell me about egypt`
- `what language do they speak in switzerland`
- `currency of kuwait`
- `population of india`
- `where is peru`
- `what country is cairo in`
- `fun fact about ireland`

It also remembers the last place you asked about, so you can use "it",
"there" or "more" instead of saying the name again:

```
YOU: what is the capital of egypt
BOT: The capital of Egypt is Cairo
YOU: tell me some info about it
BOT: Cairo is a city in Egypt. It is the biggest city in the Arab world...
YOU: what language do they speak there
BOT: In Egypt they speak Arabic
```

That works because `lastCountry` and `lastCity` hold whatever was found
last. Questions only a country can answer, like language or currency,
use the country, and everything else uses the city.

Adding a new country is one line in the `countries` list:

```js
{ names: ["iceland"], title: "Iceland", capital: "Reykjavik", continent: "Europe",
  people: "about 400 thousand", money: "Icelandic Krona", language: "Icelandic",
  flag: "IS", fact: "It has no mosquitoes at all" },
```

If a place has more than one name, put them all in `names`, like
`["usa", "america", "united states"]`. The longest name always wins, so
`south korea` beats `korea`.

## What else it knows about

Coding (HTML, CSS, JavaScript, Python, Java, C++, SQL, Git, variables, loops,
arrays, functions, APIs), science (gravity, DNA, atoms, planets, the human
body, electricity), maths (pi, primes, areas, algebra), world facts (biggest
country, longest river, continents), plus school and study tips, jokes,
football and small talk.

## Adding more knowledge

Open the file and find the `brain` list. Add a new line like this:

```js
{ keys: ["pizza"], answer: "Pizza is the best food ever 🍕" },
```

That's it, now Elhadaba knows about pizza.
