# work-cli

Awesome command line tools for managing the lifecycle of Github pull requests.

```
$ work -h

Remove every day developer toil around Github, branches, and reviews.

USAGE
  work <command> <subcommand> [flags]

CORE COMMANDS
  begin:   Create a new pull request off origin/main
  pr:      Switch between and view your pull requests
  review:  Quickly request a review and edit your PR description in one shot

ONBOARDING COMMANDS
  setup:   One-time setup to install required dependencies

FLAGS
  -h    Show help for any command

EXAMPLES
  $ work begin              # create a new PR
  $ work review cindy       # request a review from @cindy on Github
  $ work pr switch          # quick switch to another PR's branch
  $ work pr show            # quick open your PR in Chrome

LEARN MORE
  Use 'work <command> <subcommand> -h' for more information about a command.
```

## Installation

⏰ I'm busy, can I paste in 1 line of shell code?

```bash
bash <(curl -s https://raw.githubusercontent.com/dbalatero/work-cli/main/bin/install)
```

🤓 I'm paranoid about running code directly from curl:

```bash
git clone https://github.com/dbalatero/work-cli.git ~/.work-cli

cd ~/.work-cli
bin/install       # don't forget to audit the script, you nerd
```
