

# Steps to install on Mac

## Add python virtual env

- Install pyenv using Homebrew

```brew install pyenv```

- Install Python 3.11 (or 3.12)

```pyenv install 3.11.7```

- Set it as your global default

```pyenv global 3.11.7```

- Add to your shell profile (~/.zshrc or ~/.bash_profile)
```shell
echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

- Reload your shell
```shell
source ~/.zshrc
```

## Install libraries for MCP Server

```
# Create a virtual environment
python3 -m venv your_folder

# Activate it
source your_folder/bin/activate

# Now install your libraries
pip install wikipedia wikipedia_sections mcp

```

## Install libraries for MCP Client

```
pip install langchain
pip install langgraph
pip install langchain-openai
pip install langchain-mcp-adapters
```