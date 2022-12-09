# L7 Tools

## Deskripsi

[L7 Tools] merupakan perkakas cli untuk melakukan konfigurasi sistem seperti pembaruan, chroot mode, memasang grub, memperbaiki boot order, memasang pengguna baru dan lain-lain.

- Memperbarui sistem agar menjadi lebih baru.

  ```
  doas l7-tools --upgrade
  ```

  Atau menjalankan

  ```
  upgrade
  ```

- Memasang grub.

  ```
  l7-tools --grub
  ```

- Masuk ke mode chroot, berguna untuk memperbaiki jika ada kernel panic atau masalah lainnya.

  ```
  l7-tools --chroot
  ```

- Memperbaiki screen tearing dan menampilakan grub menu sistem operasi lain.

  ```
  l7-tools --patch
  ```

- Memasang pengguna baru, berguna untuk mengatasi gagal login.

  ```
  l7-tools --user
  ```

- Menghapus perangkat lunak yang tidak dibutuhkan.
  ```
  l7-tools --downgrade
  ```

Untuk menjalankan perintah diatas memerlukan akses root (doas/sudo). Lebih jelasnya jalankan `l7-tools --help`.
  ```
  ➜  ~ l7-tools --help

  LangitKetujuh Tools <version>
  Configuring tool for upgrade, chroot and grub installer.

  license : GPL-3.0-or-later
  usage   : l7-tools [option]
  option  :
            --chroot      -c    enter chroot mode
            --downgrade   -d    downgrade & uninstall program
            --grub        -g    install grub
            --patch       -p    reinstall patch
            --remote      -r    terminal remote
            --upgrade     -u    upgrade system
            --user        -m    create new user
            --help        -h    show this help
            --version     -v    show l7-tools version
  ```

[L7 Tools]:https://gitlab.com/langitketujuh/l7-tools/
