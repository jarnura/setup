Install zsh and oh-my-zsh

```
Go to root user: su -
Enter root user password

apt install zsh

which zsh

chsh -s /usr/bin/zsh root

Logout from root user

echo $SHELL  -- to check

Install wget and git

apt install wget git

wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh

cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc

source ~/.zshrc

```

Install nvim

```
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:neovim-ppa/stable
sudo apt-get update
sudo apt-get install neovim

```

Install tmux

```
sudo apt install tmux

```

Make zsh default shell

```
chsh -s $(which zsh)

```

Read the blog https://www.hamvocke.com/blog/a-guide-to-customizing-your-tmux-conf/

clone zsh auto suggestions for zsh and oh-my-zsh

To enable rename panels in tmux

```
DISABLE_AUTO_TITLE=true

paste it ~/.zshrc

```

To highlighting auotsuggestions inside tmux

```
echo  "export TERM=xterm-256color" >> ~/.zshrc

source ~/.zshrc

```

Install Vim-plug

```
Create dir ~/.config/nvim/

mkdir .config/nvim

Create ~/.vimrc flie

ln -s ~/.vimrc ~/.config/nvim/init.vim

curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

In ~/.vimrc replace call plug#begin() path with ~/.config/nvim/plugged

```




