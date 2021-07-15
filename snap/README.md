# SNAP
[Click here to go to the official tutorial to install snap on mint.](https://snapcraft.io/docs/installing-snap-on-linux-mint)

Mint has a rule that needed to be removed:

```sh
https://snapcraft.io/docs/installing-snap-on-linux-mint
```

After this you can simply do:

```sh
sudo apt update && sudo apt install snapd
```

To test do:

```sh
snap install hello-world
hello-world
```
If terminal returns a:

> Hello World!

Them its done!