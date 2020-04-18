# Panoptes

[![Build Status](https://travis-ci.org/jamesdobson/panoptes.svg?branch=master)](https://travis-ci.org/jamesdobson/panoptes)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjamesdobson%2Fpanoptes.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjamesdobson%2Fpanoptes?ref=badge_shield)

Panoptes is a mac screensaver that rotates through a set of webpages. It's ideal
for displaying status or system monitoring dashboards as your screensaver.

## Installation

Install from the [homebrew tap](https://github.com/jamesdobson/homebrew-panoptes):

```console
~ % brew tap jamesdobson/panoptes
~ % brew cask install panoptes
```

## Configuration

Panoptes currently supports configuration via the command line.

### Configuring from the CLI

Panoptes can be configured from the command line.

#### List of URLs

Get the List of URLs like this:

```console
~ % defaults read ~/Library/Containers/com.apple.ScreenSaver.Engine.legacyScreenSaver/Data/Library/Preferences/ByHost/com.softwarepunk.Panoptes urls
(
    "https://www.apple.com"
)
~ %
```

Set the list of URLs:

```console
~ % defaults write ~/Library/Containers/com.apple.ScreenSaver.Engine.legacyScreenSaver/Data/Library/Preferences/ByHost/com.softwarepunk.Panoptes urls -array "https://www.apple.com" "https://www.google.com"
~ %
```

#### Rotation Interval

The rotation interval is the time, in seconds, to display a URL before switching to a new URL.

Get it like this:

```console
~ % defaults read ~/Library/Containers/com.apple.ScreenSaver.Engine.legacyScreenSaver/Data/Library/Preferences/ByHost/com.softwarepunk.Panoptes intervalSecs
60
~ %
```

Set it like this:

```console
~ % defaults write ~/Library/Containers/com.apple.ScreenSaver.Engine.legacyScreenSaver/Data/Library/Preferences/ByHost/com.softwarepunk.Panoptes intervalSecs -float 30.0
~ %
```

## License

Licensed under the [MIT](https://github.com/jamesdobson/panoptes/blob/master/LICENSE) license.


[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjamesdobson%2Fpanoptes.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjamesdobson%2Fpanoptes?ref=badge_large)