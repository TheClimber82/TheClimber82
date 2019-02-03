If you encounter any error such as:

`error: vim-runtime: signature from "Arch Linux ARM Build System <builder@archlinuxarm.org>" is unknown trust
:: File /var/cache/pacman/pkg/vim-runtime-8.1.0022-1-aarch64.pkg.tar.xz is corrupted (invalid or corrupted package (PGP signature)).
Do you want to delete it? [Y/n] `

You can run these command to solve the issue:

`# pacman-key --init # pacman-key --populate archlinuxarm`

For more info, see here: [https://archlinuxarm.org/forum/viewtopic.php?f=65&t=12796](https://archlinuxarm.org/forum/viewtopic.php?f=65&t=12796)