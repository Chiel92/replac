# replac
Fastest CLI to do cross-platform perl regex search and replace in a git repository.

## Recommended Installation
- Install `perl` and `git` and make them available in the `PATH`.
- Add the following line to your `.bashrc`: ```alias replac="perl ~/dotfiles/replac/replac.pl"```

## Usage
```
$ replac --help
USAGE: replace <FIND_PATTERN> <SUBSTITUTE_PATTERN> [<ARBITRARY GIT GREP PARAMETERS>] [--now]

The patterns are treated as Perl regex patterns and the other arguments
are treated like the corresponding grep arguments.
If the "now" flag is not given, replace will run in dry mode

EXAMPLE:
replace "number:(\d)" "digit:$1" ../libs -- \*.{cpp,h} --now
```

## Example
