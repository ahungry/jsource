# J (APL-like)

Thanks to http://www.jsoftware.com/source.htm for open sourcing this
wonderful software!

# Building / Repo Cloning

## GNU/Linux
As tested under Arch Linux.

The build process assumes some files are in specific locations, so do
the following:

```sh
export $BUILD_TARGET=j64
cd ~
mkdir -p ~/jbld/$BUILD_TARGET/bin
mkdir ~/gitdev
git clone https://github.com/ahungry/jsource.git ~/gitdev/jsource
ln -s ~/gitdev/jsource/make/jvars.sh ~/jvars.sh
~/gitdev/jsource/make/build_all.sh $BUILD_TARGET

# At this point, everything should be built, so run with:
~/jbld/j64/bin/jconsole
```

# License

GPLv3 or Later
