# larskghf/homebrew-tap

Personal Homebrew tap for tools maintained by [larskghf](https://github.com/larskghf).

## Available formulae

### [clawdstacc](https://github.com/larskghf/clawdstacc)

Self-hosted Codespaces for Claude Code, on your own Mac. Persistent
`claude --rc` sessions per project, watchable from a tiny live dashboard,
reachable from the Claude iOS/Android app as a Remote Control session.

```bash
brew tap larskghf/tap
brew install clawdstacc

# First-time setup
cp $(brew --prefix)/etc/clawdstacc/clawdstacc.conf.example ~/clawdstacc.conf
$EDITOR ~/clawdstacc.conf
clawdstacc setup --conf ~/clawdstacc.conf
```

The Claude Code CLI is not on Homebrew — install separately:

```bash
curl -fsSL https://claude.com/install.sh | bash
```

## How it works

`Formula/clawdstacc.rb` is generated and pushed automatically by
[GoReleaser](https://goreleaser.com) on every tagged release of the
[clawdstacc](https://github.com/larskghf/clawdstacc) repo. Don't edit
the formula by hand — your changes will be overwritten on the next
release.

## License

Each formula in this tap follows its source project's license.
