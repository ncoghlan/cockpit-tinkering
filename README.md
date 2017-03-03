# cockpit-tinkering
Tinkering repo to learn about how to create Cockpit plugins

## Source articles:

* http://stef.thewalter.net/creating-plugins-for-the-cockpit-user-interface.html
* http://stef.thewalter.net/using-dbus-from-javascript-in-cockpit.html

To get the zoner demo to work from a sudo-enabled account, make sure to check
the "Reuse password for privileged operations" box when logging in.

## Adding to Cockpit as user plugins

    $ mkdir -p ~/.local/share/cockpit
    $ ln -snf $PWD/pinger ~/.local/share/cockpit/pinger
    $ ln -snf $PWD/zoner ~/.local/share/cockpit/zoner

## Adding to Cockpit as system plugins

    $ sudo ln -snf $PWD/pinger /usr/share/cockpit/pinger
    $ sudo ln -snf $PWD/zoner /usr/share/cockpit/zoner
