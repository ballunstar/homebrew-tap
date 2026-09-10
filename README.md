# ballunstar/homebrew-tap

```bash
brew install ballunstar/tap/vibewidget
vibewidget-refresh
```

[VibeWidget](https://github.com/ballunstar/vibe-widget) is a macOS menu bar app
and widget showing how much Claude and Codex usage is left. macOS 14 or newer.

Nothing compiles and nothing is signed on your machine: the release ships an
already-signed universal bundle, so no Xcode and no Apple ID are needed.
`vibewidget-refresh` is the second half of the install — it places the app in
`~/Applications` and tells macOS about the widget, which Homebrew is not allowed
to do itself. Run it again after every upgrade.

There is no `brew tap` step. Naming the formula in full is what tells recent
Homebrew you trust it; tapping the whole tap first is what gets refused.

`Formula/vibewidget.rb` is written here by `Tools/release.sh` in the app's own
repository. Edit it there, not here.
