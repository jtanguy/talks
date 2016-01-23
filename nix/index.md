---
layout: ribbon
style: |
    .slide:after {
        display: none;
    }
    #Cover {
        background: url("pictures/cover.jpg");
        background-size: cover;
        color:#FFF;
    }
    #Cover h2 {
        margin:30px 0 0;
        color:#FFF;
        text-align:center;
        font-size:70px;
        }
    #Cover p {
        margin:10px 0 0;
        text-align:center;
        color:#FFF;
        font-style:italic;
        font-size:20px;
        }
        #Cover p a {
            color:#FFF;
            }
    #Picture h2 {
        color:#FFF;
        }
    #SeeMore h2 {
        font-size:100px
        }
    #SeeMore img {
        width:0.72em;
        height:0.72em;
        }
---

# Nix, a declarative package manager {#Cover}

*By [Julien Tanguy](http://twitter.com/jutanguy)*

## **Managing systems is hard**

## Trying out software

### Install

- The easy way: `<package manager> install`
- The hard way: `./configure`, `make`, `make install`
- The YOLO way: `curl <url> | sudo bash`

### Uninstall

- `<package manager> uninstall`

## **Multiple versions of the same package is hard**

## One problem: the FHS

- `/bin`: binaries
- `/opt`: software installed system-wide using automatic installers
- `/etc`: system-wide configuration files
- `/lib`: libraries
- `/usr`: kitchen sink

## Solutions

- Per-language sandboxes: virtualenv, rvm, nvm, stack
- Containers

## **Nix**

## Derivations

- Small building block
- Derived explicitly from each other

## `/nix/store`

TODO: ls /nix/store | head -n 10

## Anatomy of a derivation

TODO: ls /nix/store/something

## Reproducible builds

- Gratuitous variables are set to their mathematical equivalent of zero
  - time/date
  - environment
  - non-essential file system contents (the build is chrooted)

- All essential variables (called build inputs) count into the hash:
  - build toolchain – compiler / linker / etc.
  - other build time dependencies – kernel headers, libc, libraries, make, automake, coreutils
  - runtime dependencies


## Profiles
{:.cover #Profiles}

![](pictures/user-environment.png)
<!-- Image from http://nixos.org/nix/manual/#sec-profiles -->

## **Killer feature: `nix-shell`**

## References

- [Knowing your system, pt.1 -- @Keruspe](http://www.imagination-land.org/posts/2012-11-22-knowing-your-system-part-basics-on-unixlike-systems.html)
