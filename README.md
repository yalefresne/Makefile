# Makefile for Symfony project

![](https://badgen.net/badge/icon/github/black?icon=github&label)
![](https://badgen.net/badge/sf/symfony/green)
![](https://badgen.net/badge/icon/docker?icon=docker&label)
![](https://badgen.net/badge/icon/yarn/cyan?icon=npm&label)

This file will improve over time. Don't hesitate to add a comment, create an issue or whatever you want, if you have a question or just want to discuss or give me some advice. 
 
If you're working on a Symfony project, in Docker container. This makefile can be useful for you. If not, it can be an inspiration for your project. 
I myself was inspired by [@COil](https://github.com/COil) and his [article that i recommend to you](https://www.strangebuzz.com/en/blog/setting-a-ci-cd-workflow-for-a-symfony-project-thanks-to-the-github-actions)

Add this make file in your project and let's go, customize it as you need.

You can run `make` command to see list of available command.
It will print something like that:

```
help                           Outputs this help screen
 —————— Initialize Project 🚀 ———————————————————————————————————————————————
init                           Initialize the project
 —————— Config Github ⚙️  ————————————————————————————————————————————————————
gc                             Config path to Github hook
 —————— Docker 🐳 ———————————————————————————————————————————————————————————
up                             Start the docker hub
docker-build                   UP+rebuild the application image
down                           Stop the docker hub
 —————— Composer 🧙‍♂️ —————————————————————————————————————————————————————————
install                        Install vendors according to the current composer.lock file
update                         Update vendors according to the composer.json file
require                        Followed by package name to add it.
reqdev                         Followed by package name to add it in require-dev.
 —————— Yarn 🧶 —————————————————————————————————————————————————————————————
ynstall                        Install node modules according to current package.json file
add                            Followed by package name to add it.
addev                          Followed by package name to add it in devDependencies.
 —————— Symfony 🎵 ——————————————————————————————————————————————————————————
sf                             List all Symfony commands
cc                             Clear the cache
warmup                         Warmup the cache
purge                          Purge cache and logs
 —————— Doctrine ▶️ ——————————————————————————————————————————————————————————
dgm                            Generate a blank migration class
dmm                            Execute migrations
 —————— Coding standards ✨ —————————————————————————————————————————————————
cs                             Executes php cs fixer
 —————— Tools 🔧 ————————————————————————————————————————————————————————————
bp                             Bash into php container
bn                             Bash into node container
```
