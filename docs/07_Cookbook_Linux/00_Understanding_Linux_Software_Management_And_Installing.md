## Overview

In this tutorial we'll take [Ubuntu](https://www.ubuntu.com/) as example.
Ubuntu, a linux based operating system, handles software management in a way you may not be used to. It is however, very convenient at the end of the day. Ubuntu features a repository system, which is a software collection stored on several servers, which you can access and install with few commands.
This ensures that updating and installing software is easy, efficient and safe.

To quote from [Wikipedia](https://en.wikipedia.org/wiki/Package_manager):

> In software, a package management system, also called package manager, is a collection of software tools to automate the process of installing, upgrading, configuring, and removing software packages for a computer's operating system in a consistent manner. It typically maintains a database of software dependencies and version information to prevent software mismatches and missing prerequisites.
>Packages are distributions of software, applications and data. Packages also contain metadata, such as the software's name, description of its purpose, version number, vendor, checksum, and a list of dependencies necessary for the software to run properly. Upon installation, metadata is stored in a local package database.

Ubuntu integrated software manager is a command-line tool called apt. Using it is very straight forwarding. Apt has it’s own repository list, stored in

    /etc/apt/sources.list

You can add or remove software sources by editing this file. To see its content just type:

    cat /etc/apt/sources.list


It is however suggested to edit this only if you know what you are doing.

Before attempting to install a software from a repository, let’s update the apt cache. This is basically a database of all available software, that includes [dependencies](https://en.wikipedia.org/wiki/Coupling_(computer_programming)) and version informations.

To update:

    sudo apt update

Then, let’s assume we want to install nano, a very useful and simple text-editor:

    sudo apt install nano


We will be asked if we wish to continue, let’s reply yes. So, type `y`

Apt will then download, unpack and install all file needed for us. Just wait a while and it will finish.

Let’s assume then, we want to remove a program, for example vim (another text-editor)

    sudo apt remove vim


Again, we reply yes typing `y`.

## Some other useful commands for apt, and system housekeeping, are:

    apt autoremove

removes automatically packages that are no longer required

    apt clean


deleted downloaded packages that are wasting disk space

We can now use another package manager, with a graphical user interface, Synaptic, which is the default package manager in most Ubuntu versions.

We’ll use apt to install synaptic

    apt install synaptic


Once installed, we’ll find Synaptic Package Manager in the “Other” applications menu. Let’s open it.

Type your root password, and enter.

You can then, search and install every package you like, in a nice and user friendly environment.

To start, we will enable more software sources than we have by default.

To do this, go to `settings` then `repositories` and check all the repositories you wish to enable; typically you should be good enabling all software sources from the “Ubuntu Software” tab.

Once done, close and hit `reload`, which is the same as `apt update`.

When finished, you can start searching and browsing for thousands of different softwares, to install them simply tick the checkbox, select `Mark for installation` and hit `apply`.

You have now at your disposal all the software you need to further expand UDOO VISION capabilities.