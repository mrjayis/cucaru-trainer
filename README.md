# Cucaru trainer

Practice Cucaru against computer players in the browser: https://mrjayis.github.io/cucaru-trainer/

Cucaru is a double-board PLO game. Everyone antes, two flops are dealt, and each
player makes one decision, starting with the small blind and ending on the
button: put in the amount of the pot (the total of the antes) or fold. There is
no raising and no action on the turn or river. Each board wins half the pot, and
ties split.

- PLO4, PLO5 or PLO6, with 2 to 10 players (fewer players for 5- and 6-card hands, so the deck doesn't run out)
- Pot odds and your equity against the live field, each of which can be turned on or off
- Bots put money in when their equity against the live field beats the average share (1 / players still in)
- After each hand: exact flop equity against the hands that went in, EV next to your result, and a session log

A single self-contained `index.html` with no build step. The hand evaluator is
the integer evaluator from the PLO DBBP equity engine, extended to 5- and
6-card hands.
