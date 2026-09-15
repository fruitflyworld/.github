# Contributing

Thanks for looking. Issues and pull requests are welcome on any repository in
this organization.

Fruit Fly World lives in one repository —
[**fruitflyworld/fruit-fly-world**](https://github.com/fruitflyworld/fruit-fly-world) —
and that repository's
[`CONTRIBUTING.md`](https://github.com/fruitflyworld/fruit-fly-world/blob/main/CONTRIBUTING.md)
is the one that applies. Read it before you open a pull request. The short
version, because it is the part people get wrong:

- The arena rules live in **one file** that the browser and the server both
  import, and there is a plain-JavaScript copy of that file in the agent skill.
  Change one, change the other in the same commit — a parity test fails the
  build otherwise.
- If you change the scoring, the map, the energy rule or the caps, update the
  published rules in the same commit.
- `npm run check` has to pass on a clean checkout with no `.env`.

If you think you have found a vulnerability, do not open a public issue — read
[SECURITY.md](SECURITY.md) and report it privately.
