# GCI-Fedora-Silver-Blue
## Introdution
![alt text](https://github.com/Ayush19-01/GCI-Fedora-Silver-Blue/blob/master/resources/what-is-fedora-silverblue-816x345.jpg)

__Silverblue__ is a _immutable_ variant of Fedora Workstation. It is like a regular desktop operating system, you will never be
able to find the difference between the standard Fedora Workstation, the user experiences the same features with a new, yet 
different structure.

__Silverblue’s__ core technology is really helpfull as OS updates are fast and there’s no waiting around for them 
to install. It is also possible to go back to the previous version of the operating system,if something wnet wrong, 
which is perfect for developers who experiment on the OS and tend to break a couple of things during that period.
For example: If some user gets the OS to the state when it doesn’t boot or doesn’t work properly after accidentally 
or unintentionally removing some system library. It is practically impossible for that tester to do so.

The difference between Silver Blue and the OS is that the former is _immutable_. This means that operating system that is 
on one machine is exactly same as the one in any machine around the world, and it never changes as it is used.Its _immutable_ 
design makes it more stable, less prone to bugs, and easier to test and develop. Also this _immutable_ design makes it the perfect
platform for containerized apps as well as container-based software development, improving stability and reliability.

## Immutable OS

_Immutable_ infrastructure is comprised of _immutable_ components that are replaced for every deployment, rather than 
being updated in-place. Those components are started from a common image that is built once per deployment and can be
tested and validated.

As the root filesystems are mounted to read-only by default, it increases resilience against accidental damage as well as some
types of malicious attack. The primary tool to upgrade or change the root filesystem is rpm-ostree.

## Ostree

OSTree is an upgrade system for Linux-based operating systems that performs atomic upgrades of complete filesystem trees.
It is not a package system; rather, it is intended to complement them. A primary model is composing packages on a server,
and then replicating them to clients.

The underlying architecture might be summarized as "git for operating system binaries". It operates in userspace, and will
work on top of any Linux filesystem. At its core is a git-like content-addressed object store with branches (or "refs") to 
track meaningful filesystem trees within the store. Similarly, one can check out or commit to these branches.

## Working with Silver Blue

![alt text](https://github.com/Ayush19-01/GCI-Fedora-Silver-Blue/blob/master/resources/1.svg)

It's _immutable_, which means that you don't upgrade packages: you just create a new version of the operating system 
with the new packages and boot into that. You know exactly what you're running.Once you've taken new versions of packages,
you just reboot into the new version, and you're good to go. If there's a problem with it, you can revert to the old version.
Which is good for stability also for security.

If you really need a different version of an operating system package, you can layer it on top of the existing one, but 
this loses some of the benefits of the immutability. When you want to install applications, the preferred way of doing so 
is to use Flatpak.

## Finally....

If one's requirement is a stable desktop system, and particularly interested in using Flatpak, then it is highly recommended
to give __Silverblue__ a shot. Installation is easy(simpler than most linux OS's), applications are simple to get onto your 
system. Plus if you're used to Fedora workstation or any standard Linux desktop system,you wont have any problem with trying
it. It's new, stable and easy to use, why not try __Silverblue__?

### Acknowledgement

___Points extracted from:___

   ___1) https://docs.fedoraproject.org/en-US/fedora-silverblue/___
  
   ___2) https://fedoramagazine.org/what-is-silverblue/___
  
   ___3) https://ostree.readthedocs.io/en/latest/manual/introduction/___
