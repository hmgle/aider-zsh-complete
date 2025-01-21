# aider-zsh-complete

Zsh completion script for the `aider` command-line tool.

## Installation

### Step 1: Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/your-username/aider-zsh-complete.git
cd aider-zsh-complete
```

### Step 2: Install the Completion Script
Copy the `_aider` completion script to your zsh completions directory:
```bash
mkdir -p ~/.zsh/completions
cp _aider ~/.zsh/completions/
```

### Step 3: Update Your Zsh Configuration
Add the following lines to your `~/.zshrc` file:
```zsh
# Add the completions directory to fpath
fpath=(~/.zsh/completions $fpath)

# Initialize the completion system
autoload -Uz compinit
compinit
```

### Step 4: Reload Zsh Configuration
Reload your zsh configuration to apply the changes:
```bash
source ~/.zshrc
```

### Step 5: Test the Completion
Test the completion by typing `aider` followed by `Tab`:
```bash
aider <Tab>
```
You should see a list of available options and arguments.

## Contributing
If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License
This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.
