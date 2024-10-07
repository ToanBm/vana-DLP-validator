# Installation Vana DLP Validator

## Prepare enviroment
### 1. Install Python 3.11:
sudo apt update
sudo apt install software-properties-common

sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.11 python3.11-venv python3.11-dev python3-pip

python3.11 --version
### 2. Install Poetry
curl -sSL https://install.python-poetry.org | python3 -

echo 'export PATH="$HOME/.local/bin:$PATH"' >> $HOME/.bash_profile
source $HOME/.bash_profile
poetry --version

### 3. Install Nodejs & Npm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash

echo 'export NVM_DIR="$HOME/.nvm"' >> $HOME/.bash_profile
echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm' >> $HOME/.bash_profile
echo '[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion' >> $HOME/.bash_profile

source $HOME/.bash_profile

nvm install --lts

node -v
npm -v

## Setup steps
### 1. Clone Vana-dlp-chatgpt git repo
git clone https://github.com/vana-com/vana-dlp-chatgpt.git
cd vana-dlp-chatgpt
### 2. Install dependencies
poetry install
















