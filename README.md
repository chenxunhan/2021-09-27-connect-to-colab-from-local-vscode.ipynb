# TUTORIAL: Vscode connecting Colab Runtime

## easy tutorial(review if you forget the config step, or get started on the next step)
- [2021-09-27-connect-to-colab-from-local-vscode.ipynb](https://colab.research.google.com/github/JayThibs/jacques-blog/blob/master/_notebooks/2021-09-27-connect-to-colab-from-local-vscode.ipynb#scrollTo=4Nv8QdPRGaIv)
    - if your password and github_access_token are set by yourself, ignore the optional part:dotenv

## Cloudflare Installation
- [Cloudflare](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/install-and-setup/installation/)
    - download the exe file in a path
    - get the file abslute path

## get github info
- password
- email
- username
- git_repo: copy the link from your github repo that you want to edit
    - it is on the link bar in browser
- github_access_token: github/Settings/Developer settings
    - Note: token4...
    - Select scopes: all

## config github info in colab notebook and RUN
- open GPU
- [Vscode-ssh-Colab.ipynb](https://colab.research.google.com/drive/1bl1s0MMR6XPtBQ2BjXOg7bn8nVOCtfyY)
- check the output

## config ssh config
- notepad %USERPROFILE%\.ssh\config from colab output
- config ssh path in vscode(extension:Remote.SSH -> setting):
    - Remote.SSH: Config File `%USERPROFILE%\.ssh\config`
- choose remote os: linux
- choose kernel: python 3.10
