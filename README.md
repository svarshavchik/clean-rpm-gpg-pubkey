clean-rpm-gpg-pubkey
====================

A short Perl script for Fedora that removes old PGP keys from the RPM
database. Each Fedora release uses a different PGP keys, but there's
nothing in Fedora (at this time) that automatically removes prior
Fedora releases' PGP keys.

So, after updating Fedora releases, a few times, old PGP keys accumulate.
If an old PGP key was compromised (this has happened once before)
everyone needs to scramble and remove the affected PGP keys. Well, you've
already done that, so rest easy.

Nothing to install here, just download and run the script. There's a
--dry-run option that does nothing but list the affected PGP keys that
would be removed. Running the script without arguments does it for real.
