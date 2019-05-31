These are scripts that create "alternatives" for use by the Debian
`update-alternatives` program. 

The alternatives are "link groups" that get installed as a bundle
when a given master file is selected.

This particular set is for `python3`.

After installing, you can run `update-alternatives --set python3 SOMETHING`
and choose which alternative you want to serve as your python3 package.

You must have root via `su`, or be able to use `sudo`, in order to run
these scripts.

If you run as root, the scripts run `update-alternatives` directly. If
you run as not-root, the scripts run `sudo update-alternatives`.

If you can't become root, and don't have sudo access, then you can't install
alternatives. Try the `pythonz` package for managing multiple python versions
in your home directory, instead.

