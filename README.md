# Wildcard DNS

Wildcard DNS is a script to set up a wildcard localhost domain on OSX.

## What Gets Done

1. Generate RNDC key
2. Add `.dev` TLD zone to `/etc/named.conf`
3. Create the `dev.zone` file in `/var/named`
4. Start BIND

## Installation

### Default

Run this one-liner:

	bash <(curl -s https://raw.github.com/frankzilla/wildcard-dns/master/install)

### Custom

If a different TLD is required, simply clone this repo and change the `TLD` variable in the `install` file and run:

	bash < install

## More Information

Read [Setting Up Wildcard DNS on OSX](http://sqrhedz.com/post/12965056278/setting-up-wildcard-dns-on-osx) for more detailed information.