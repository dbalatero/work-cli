# work-cli

Awesome command line tools for managing the lifecycle of Github pull requests.

* Branch and open a beautiful draft PR by typing `work begin` from `main/master`
* Fast switch between your open PRs with `work pr switch`
* Open or focus your PR in the browser with `work pr show`
* Ask for a review on Github with `work review alice`

<table>
<thead>
<tr>
<th>Creating a PR</th>
<th>Result</th>
</tr>
</thead>
<tbody>
<tr>
<td valign="top" width="50%">

![image](https://user-images.githubusercontent.com/59429/197116597-fca93c73-e9e3-4e80-a524-9ab26297856c.png)

</td>
<td valign="top" width="50%">

![image](https://user-images.githubusercontent.com/59429/197116703-9291bd39-0a15-4040-b0a0-cb69127a850e.png)

</td>
</tr>
</tbody>
</table>

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

## FAQ

### I forget how to quit Vim, can I use VSCode to edit my PR descriptions?

Sure, why not. Just add this to your `bashrc/zshrc/whatever` file and reload
your shell:

```bash
export EDITOR="code --wait"
```
