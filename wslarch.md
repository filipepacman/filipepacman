https://github.com/yuk7/ArchWSL

>Arch.exe
[root@PC-NAME]# passwd

>Arch.exe
[root@PC-NAME]# echo "%wheel ALL=(ALL) ALL" > /etc/sudoers.d/wheel
(setup sudoers file.)

[root@PC-NAME]# useradd -m -G wheel -s /bin/bash {username}
(add user)

[root@PC-NAME]# passwd {username}
(set default user password)

[root@PC-NAME]# exit

>Arch.exe config --default-user {username}
    (setting to default user)

>Arch.exe

                sudo nano /etc/pacman.d/mirrorlist
[user@PC-NAME]$ sudo pacman-key --init

[user@PC-NAME]$ sudo pacman-key --populate

[user@PC-NAME]$ sudo pacman -Sy archlinux-keyring

[user@PC-NAME]$ sudo pacman -Syyuu

sudo pacman -S git base-devel wget zsh gtk4
git clone https://aur.archlinux.org/packages/libpamac-aur
makepkg -si
git clone https://aur.archlinux.org/packages/pamac-aur
makepkg -si


------------------------------------------------------------------------------------------------

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/zdharma-continuum/zinit/HEAD/scripts/install.sh)"

 code ~/.zshrc

zinit light zdharma/fast-syntax-highlighting
zinit light zsh-users/zsh-autosuggestions
zinit light zsh-users/zsh-completions