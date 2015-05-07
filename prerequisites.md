Practical Docker: Hands-on Management and Administration
========================================================

### Class Prerequisites ###

This class is for intermediate to moderately experienced Docker users. You should be familiar with the basic Docker commands and have setup and deployed Docker containers on your laptop or server.  Specific familiarity with pulling images, starting and inspecting containers and using the more common flags (-d, -it, -p, -v), and a decent understanding of Dockerfiles and how they work is important.

Generally, if you're *comfortable* with the material in the [Intro-To-Docker](https://github.com/LinuxAtDuke/Intro-To-Docker) class, you should be fine.

Unrelated to Docker, you should comfortable with the following Linux technologies:

* SSH/SCP
* Shell Scripts
* git

### Class Environment ###

You will need to bring a laptop with an SSH client installed to the class.

Sometime before class, please do the following:

1. Using a web browser, go to *https://vm-manage.oit.duke.edu*
2. Login using your Duke NetId.
3. Create a new project for this class.
4. Select *Ubuntu 14 Basic* for the Server.

The vm-manage web page will tell you the name for your VM. The web site will also tell you the initial username and password. You should connect via ssh.

Example: `ssh bitnami@colab-sbx-87.oit.duke.edu`

5. Once logged in via ssh, enter the `passwd` command to set a unique password.

Example:

    passwd
    Changing password for bitnami.
    (current) UNIX password:
    Enter new UNIX password:
    Retype new UNIX password:


6. Update Ubuntu

Example:

    sudo apt-get update && sudo apt-get upgrade

7. Install the latest version of Docker *From Docker.com*

Example:

    wget -qO- https://get.docker.com/ | sh

8. Install the latest version of Docker Compose *From Docker.com*

Example:

    curl -L https://github.com/docker/compose/releases/download/1.2.0/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
    chmod +x /usr/local/bin/docker-compose

9. Clone this repo

Example:

    git clone https://github.com/LinuxAtDuke/Practical-Docker.git

10. Sit back and have a coffee and ponder this Docker Koan: *Can anything REALLY be in a container?*

**See you in class!**
