# l4d2-dedicated-server
set up a left 4 dead 2 dedicated server on `debian` via `vagrant`, `virtualbox` and `ansible`.

# quick-and-dirty readme
- vagrant plugin install vagrant-vbguest
- vagrant up
- vagrant status
- vagrant ssh l4d2-ds-provision-vm
- vagrant ssh l4d2-ds-development-vm
- vagrant provision l4d2-ds-provision-vm
- vagrant reload

## remove
- vagrant destroy --force --parallel
- rm -R .vagrant
- rm -R ~/.vagrant.d

## steam license agreement
- by executing `vagrant up`, you are automatically accepting the `[steam license agreement](https://store.steampowered.com/agreement)`.

## connect
- console: `connect 127.0.0.42:27015`
- `bind "F3" "openserverbrowser"`

## forwarded ports
- guest "0.0.0.0:27015" (TCP) -> host "127.0.0.42:27015" (TCP)
- guest "0.0.0.0:27015" (UDP) -> host "127.0.0.42:27015" (UDP)
- [...]

## netconsole
nc 127.0.0.1 42000
