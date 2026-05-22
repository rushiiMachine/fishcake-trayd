fishcake-trayd 🍥
=================

A persistent fishcake tray icon in your system bar 🍥


Installation
------------

0. This package only has an installation script for Arch Linux and its derivatives.

1. Install this package by cloning the repository and running ``makepkg``:

   .. code-block:: shell

        $ git clone https://github.com/rushiiMachine/fishcake-trayd.git
        $ cd fishcake-trayd
        $ makepkg --install

2. If using ``gnome-shell``, install the `AppIndicator and KStatusNotification Support`_ extension, or an
   equivalent extension for your window manager. This can be done in two ways:

   2.1. Directly install the Gnome `AppIndicator and KStatusNotification Support`_ extension, and manually enable it.

   2.2. Install the ``gnome-shell-extension-appindicator`` package, and make sure to manually enable it:

   .. code-block:: shell

      $ sudo pacman -S gnome-shell-extension-appindicator

3. Enable and start the ``fishcake-trayd`` systemd service:

   .. code-block:: shell

       $ systemctl --user enable --now fishcake-trayd.service

4. You now have a fishcake 🍥 in your system tray!


.. _AppIndicator and KStatusNotification Support: https://extensions.gnome.org/extension/615/appindicator-support/
