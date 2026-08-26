If you want exactly the skull screen in your photo
That is most likely a custom Plymouth theme, rather than one of Rocky's standard themes. You would need the theme files installed under:
/usr/share/plymouth/themes/
A typical custom theme contains a .plymouth file plus images/scripts. After installing it, you would do:
sudo plymouth-set-default-theme -R THEME_NAME
sudo reboot
The -R is important because Plymouth is loaded from the initramfs during boot. �
The worst person in the world
