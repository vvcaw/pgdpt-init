# pgdpt-init
Automatically make your pgdp homework ready for testing.

# A little note
- This script is only tested on my own setup, I can't guarantee for it working on any other system!

# How it works
- Changes to the `.gitignore` and the `build.gradle` file are ignored, as dependencies are injected, therefore any changes made to these files will not show up in version control, if you wish to revert these changes, use `git update-index --no-skip-worktree .gitignore` and `git update-index --no-skip-worktree build.gradle` respectively.
- Creates a symbolic link to the directory provided to the script, therefore updating the `pgdp2223-tests` repository will also update the linked tests in your repository.

# Installation
Clone this repository
```
git clone https://github.com/vvcaw/pgdpt-init.git
```

Make the script executable & install it to `/usr/local/bin/`
```
cd pgdpt-init
chmod +x pgdpt-init
sudo cp pgdpt-init /usr/local/bin/
```

# Using the script
Go to the homework folder you want to add tests to and execute this command
```
pgdpt-init folder/to/pgdp2223-tests
```
the script will automatically get the right tests, based on which homework folder you execute this in.


# Installation & Demo (in video form)
[![asciicast](https://asciinema.org/a/Gaaewrw4GVEFM6ySGkGxPOGaQ.svg)](https://asciinema.org/a/Gaaewrw4GVEFM6ySGkGxPOGaQ)
