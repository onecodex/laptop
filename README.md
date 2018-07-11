Laptop
======

Forked from: https://github.com/thoughtbot/laptop

Set up
------

Download the script:

```sh
curl --remote-name https://raw.githubusercontent.com/onecodex/laptop/master/mac && curl --remote-name https://raw.githubusercontent.com/onecodex/laptop/master/laptop.local
```

Review the script (avoid running scripts you haven't read!):

```sh
less mac
```

Modify and review your `laptop.local` script as desired, then move to `~/.laptop.local`

```sh
less laptop.local
mv laptop.local ~/.laptop.local
```

Execute the downloaded script:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

Optionally, review the log:

```sh
less ~/laptop.log
```

Optionally, [install thoughtbot/dotfiles][dotfiles], and delete the `mac` script:

```sh
rm mac
```

Debugging
---------

Your last Laptop run will be saved to `~/laptop.log`.
Read through it to see if you can debug the issue yourself.
If not, copy the lines where the script failed into a
[new GitHub Issue](https://github.com/thoughtbot/laptop/issues/new) for us.
Or, attach the whole log file as an attachment.

What it sets up
---------------

All of the tools from [thoughtbot/laptop](https://github.com/thoughtbot/laptop), plus `python`, `pyenv`, `node`, and `rustup` and `rust` (including nightly).