---
layout: default
---

## jgeboski's Software Packages

As of **April 7, 2016**, the following repositories have moved:

  - `jgeboski/bitlbee-facebook` -> `bitlbee/bitlbee-facebook`
  - `jgeboski/bitlbee-steam` -> `bitlbee/bitlbee-steam`
  - `jgeboski/purple-facebook` -> `dequis/purple-facebook`

As of **April 4, 2016**, [@dequis][p2] is the new maintainer of the
Facebook related projects. The Facebook related packages will cease
to exist in [@jgeboski][p1]'s repository in the near future, please
switch to the updated repositories once they are available (this page
will be updated with the new repositories).

This is an informational page on the software packages developed by
[@jgeboski][p1]. This page retains a list of actively maintained
software packages, along with some package repositories.

[p1]: https://github.com/jgeboski
[p2]: https://github.com/dequis

## Software Packages

Below are a list of packages which I develop and maintain.

| Package                | Description                             |
|------------------------|-----------------------------------------|
| [bitlbee-facebook][s1] | Facebook protocol plugin for BitlBee.   |
| [bitlbee-steam][s2]    | Steam protocol plugin for BitlBee.      |
| [purple-facebook][s3]  | Facebook protocol plugin for libpurple. |

[s1]: https://github.com/bitlbee/bitlbee-facebook
[s2]: https://github.com/bitlbee/bitlbee-steam
[s3]: https://github.com/dequis/purple-facebook/wiki

## Package Repositories

Below are a list of instructions for installing binary packages on
various *NIX distributions. All binary packages are built using the
[openSUSE Build Service][l1].

[l1]: https://build.opensuse.org/project/show/home:jgeboski

### Debian and Ubuntu

| Release Name            | Release Version | Version         |
|-------------------------|-----------------|-----------------|
| Debian Wheezy           | 7.0             | `Debian_7.0`    |
| Debian Jessie           | 8.0             | `Debian_8.0`    |
| Ubuntu Precise Pangolin | 12.04           | `xUbuntu_12.04` |
| Ubuntu Trusty Tahr      | 14.04           | `xUbuntu_14.04` |
| Ubuntu Utopic Unicorn   | 14.10           | `xUbuntu_14.10` |
| Ubuntu Vivid Vervet     | 15.04           | `xUbuntu_15.04` |
| Ubuntu Wily Werewolf    | 15.10           | `xUbuntu_15.10` |
| Ubuntu Xenial Xerus     | 16.04           | `xUbuntu_16.04` |

1. Add the following line to `/etc/apt/sources.list.d/jgeboski.list`:

   ```
   deb http://download.opensuse.org/repositories/home:/jgeboski/<version> ./
   ```

   Notes:

   1. Replace `<version>` with your version from the table above.
   2. The `jgeboski.list` file will likely not exist.

2. Add the repository key:

   ```
   $ wget -O- {{ site.url }}/obs.key | sudo apt-key add -
   ```

3. Update the package index:

   `$ sudo apt-get update`

4. Install the plugin:

   `$ sudo apt-get install <package>`

   Notes:

   1. Replace `<package>` with a package name from the table above.
   2. The `bitlbee` packages must be used with the [nightly][r1] repository.

[r1]: http://code.bitlbee.org/debian/
