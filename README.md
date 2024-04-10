### Coinbase 

- A Vue Coinbase project built with Vue 3, TypeScript, TailwindCss, heroicons/vue, millify and vue3-smooth-scroll. 
- This project is a similar froontend like Coinbase and will enable you to learn how to use Rapid Api to fetch data from one of its huge collection of APIs.

#### Install

- Server -> Debian fork ubt 20x

- Install Yarn 

``` curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - ```

``` echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list ```

``` sudo apt update ```

``` sudo apt install yarn ```

- The command above will also install Node.js . If you installed Node trough nvm, skip the Node.js installation with:

``` sudo apt install --no-install-recommends yarn ```

- If you don thave nvm use the following --> https://heynode.com/tutorial/install-nodejs-locally-nvm

``` curl -sL https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh -o install_nvm.sh ```

``` bash install_nvm.sh ```

``` source ~/.bash_profile ```

``` export NVM_DIR="$HOME/.nvm" ```
``` [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm ```
``` [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion ```

``` nvm use ``` # there is a .nvmrc that you can use ^_^ ver 16.14

``` yarn ``` # Installs Dependencies

``` yarn dev ``` Starts the App

Install pm2 for fork process on shell ``` npm install pm2 -g ```

``` start with pm2 --name Tornado start dev -- dev ```

#### Troubleshooting

- Error: ENOSPC: System limit for number of file watchers reached

``` echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p ```