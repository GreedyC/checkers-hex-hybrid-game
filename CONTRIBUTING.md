# Contributing

Thank you for your interest in Checkers + Hex! Contributions of every size are welcome — a typo fix, a bug report, a new agent, or a whole new idea.

This repository is **v1, frozen**. The live game at <https://checkers-hex.nazakgul.games> has moved on since. v1 stays here so anyone can build on it, so forks and experiments are very welcome.

## Ways to help

- Report a bug or an unclear game state (screenshots help a lot)
- Point out where the rules text is ambiguous
- Improve accessibility, the UI, or browser support
- Write a smarter agent, or tooling to run agent-vs-agent games
- Improve replay and logging
- Add tests for the rules engine
- Pick something from [docs/IDEAS.md](docs/IDEAS.md)

## How to contribute

1. Fork the repository and create a branch.
2. Make your change.
3. Test it by opening `index.html` in a browser (no install needed). If you add tests, run `npm test`.
4. Open a pull request saying what changed and why.

Not sure where to start? Open an [issue](https://github.com/comoyomalove/checkers-hex-hybrid-game/issues) and ask.

## Proposing a rule change

The design follows one principle: **inherit, don't invent**. Rules come from Checkers or Hex wherever possible; new rules are added only when the two parents cannot combine. If you propose a change, please include:

- the current rule
- the proposed rule
- which parent it comes from (or why a new rule is needed)
- an example board situation, if relevant

## Please don't commit

Secrets, `.env` files, credentials, or personal files.

## Licence

By contributing, you agree your contribution is released under the [MIT License](LICENSE) of this project.

## Code of conduct

Everyone taking part is expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
