Ansible roles: github_easy_maintenance settings
===

# Overviews

Github_easy_maintenance is [this repository](https://github.com/gano2018/bash_github_easy_maintenance)
This roles makes setting for using this repository, git clone and github_token_setting and so on.

## Setup

### 1. Get the api token

Get the api access token for Github from [this page](https://github.com/settings/tokens) and put somewhere on your computer.

### 2. Put the file contains api access token

Put the file contains api access token anywhere you want.

### 3. Edit the defaults/main.yml.default

Copy defaults/main.yml.default as defaults/main.yml

Change the main.yml to your information as below.

  ```
  #! /bin/sh
  access_token_dir: 'where_you_put_github_access_token'  # -> the place you put the token file
  github_user: 'github_username'                         # -> your github username
  key_comment: 'key_comment_for_keygen'                  # -> key comment for keygen command
  user: 'username_who_execute_shell'                     # -> who uses the shell command
  ```

## Usage

Executing the roles, you can use 4 new shell explained in [this page](https://github.com/gano2018/bash_github_easy_maintenance)

But, you may need to `sudo` when executing the shells because of permission for github token access. If you don't like that, please change the permission for access to github api token.
