# vagrant-mono

![MonoDevelop](https://upload.wikimedia.org/wikipedia/commons/f/ff/MonoDevelopLogo.png)

## Description

A [Vagrant] setup to use [Mono] with [Debian Jessie 8.1.0 Release x64](https://www.debian.org/releases/stable/)

**Table of Contents**

- [Quickstart](#quickstart)
- [License](#license)

## Quickstart

First clone the repository:

```
$ cd ~/workspace/
$ mkdir mono
$ git clone https://github.com/ivan-iver/vagrant-mono.git
```

After that you can run your vagrant machine:

```
$ cd mono/
$ vagrant up --provision
```

Then the box will be downloaded for you.

If you wish, you can learn more about it alter a [vagrant file](Vagrantfile) and its [configuration options](ConfigOptions).

## Copyright and license

***

Copyright (c) 2015 Iván Jaimes. See [LICENSE](LICENSE) for details.

[Vagrant]: http://www.vagrantup.com/
[Mono]: http://www.mono-project.com/
[Vagrantfile]: https://github.com/ivan-iver/vagrant-mono/blob/master/Vagrantfile
[ConfigOptions]: http://docs.vagrantup.com/v2/vagrantfile/
