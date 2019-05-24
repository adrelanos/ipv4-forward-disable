# Deactivates IPv4 forwarding using /etc/sysctl.d/ #

IPv4 forwarding is not required for a Tor based Anonymity Distribution
Gateways. Deactivating it as defense in depth to prevent leaks.

For better security.
## How to install `ipv4-forward-disable` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `ipv4-forward-disable`.

```
sudo apt-get install ipv4-forward-disable
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `ipv4-forward-disable` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`ipv4-forward-disable` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
