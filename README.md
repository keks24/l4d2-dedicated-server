# l4d2-dedicated-server
set up a left 4 dead 2 dedicated server on `debian` via `vagrant`, `virtualbox` and `ansible`.

# quick-and-dirty readme
- vagrant plugin install vagrant-vbguest
- vagrant up
- vagrant status
- vagrant ssh l4d2-ds-provision-vm
- vagrant ssh l4d2-ds-development-vm

## remove
- vagrant destroy --force
- rm -R .vagrant
- rm -R ~/.vagrant.d

## steam license agreement
by executing `vagrant up`, you are automatically accepting the `[steam license agreement](https://store.steampowered.com/agreement)`.
