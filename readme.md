About
================================================================================

A deployment bootstrap script for setting up Python environment tasks like
installing setting up a virtualenv and importing requirements.txt into pip. Can
be run multiple times, it is written to be idempotent.

The main `setup.sh` script contains commonly needed functionality for all
types of projects.

Application specific setup scripts should go in the `setup/` directory. Files
are executed in alphabetical order. They can be any kind of file, with any kind
of file extension. The only requirement is the file is executable using `$
source setup/file.name` syntax. Since files are executed using `source` all
bash environment variables in `setup.sh` are available in bash `setup/`
scripts.


License
================================================================================

All code written by me is released under MIT license. See the attached
license.txt file for more information, including commentary on license choice.
