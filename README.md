# homebrew-tap (example)

Example [Homebrew](https://brew.sh/) **tap** for use with [foss-template](https://github.com/adamsiwiec1/foss-template).

## Why this repo exists

Homebrew only installs formulae/casks from a **tap** (a GitHub repo named
`homebrew-tap` or `homebrew-<name>`). Your application repository cannot serve
as the tap. Release CI pushes updated `Casks/*.rb` files here.

Production reference: [openhat-security/homebrew-tap](https://github.com/openhat-security/homebrew-tap).

## Layout

```
Casks/
  your-cli.rb    # one cask per CLI
```

Template cask: [`foss-template/packaging/homebrew`](https://github.com/adamsiwiec1/foss-template/tree/main/packaging/homebrew).

## Users

```bash
brew install --cask adamsiwiec1/tap/INSERT_REPO
```

(`adamsiwiec1/tap` is Homebrew shorthand for `adamsiwiec1/homebrew-tap`.)
