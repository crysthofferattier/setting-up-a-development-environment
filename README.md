# Setting up a Development Environment
Setting up a web/mobile development environment in a Linux distribution.

## Getting Started
[Ubuntu](https://www.ubuntu.com/download/desktop) - Ubuntu 16.04.1 LTS

### Prerequisites
* Basic command line knowledge in Linux
* Internet connection

## Built With

* [Nvidia](http://www.nvidia.com.br/graphics-cards/geforce/pascal/br/gtx-1050) - Nvidia driver
* [Ubuntu Restricted Extras](https://en.wikipedia.org/wiki/Ubuntu-restricted-extras) - Software package for the computer operating system Ubuntu
* [Curl](https://www.java.com/pt_BR/) - Java SE Development Kit 9
* [Java](https://www.java.com/pt_BR/) - Java SE Development Kit 9
* [PHP](https://secure.php.net/) - PHP 7.0
* [NodeJS](https://nodejs.org/en/about/) - NodeJS 8.x LTS
* [Composer](https://getcomposer.org/) - Dependency Manager for PHP
* [MySql](https://www.mysql.com/) - MySql server
* [NPM](https://www.npmjs.com/) - Package manager for JavaScript
* [Git](https://git-scm.com/) - Version control system
* [Sublime Text](https://www.sublimetext.com/) - Sublime Text is a sophisticated text editor for code, markup and prose
* [VirtualBox](https://www.virtualbox.org/) -  Virtualization product
* [PhpStorm](https://www.jetbrains.com/phpstorm/) - IDE for PHP development
* [Eclipse](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/oxygen2) - IDE for Java development

## Installation Guide
This installation guide provides instructions on how to manually install and configure software on a web server.


### Nvidia v384

```
$ sudo apt-get install nvidia-384 nvidia-modprobe
```

### Ubuntu Restricted Extras

```
$ sudo apt-get install ubuntu-restricted-extras
```

### Curl v7.47.0

```
$ sudo apt-get install curl
```

### Java v9.0.4

```
$ sudo add-apt-repository ppa:webupd8team/java
$ sudo apt-get update
$ sudo apt-get install oracle-java9-installer
$ sudo apt-get install oracle-java9-set-default
```

### PHP v7.0.22

```
$ sudo apt-get install php7.0
```

### NodeJS v8.9.4

NodeJS installation guide [link](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)

```
$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
$ sudo apt-get install -y nodejs
$ sudo apt-get install -y build-essential
```

### Composer v1.6.3

Composer installation guide [link](https://getcomposer.org/download/)

```
$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
$ php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ php composer-setup.php
$ php -r "unlink('composer-setup.php');"
$ mv composer.phar /usr/local/bin/composer
```


### MySQL v5.7.21

```
$ sudo apt-get install mysql-server
$ mysql_secure_installation
```

### Git v2.7.4

Git installation guide [link](https://git-scm.com/download/linux)

```
$ sudo apt-get install git
```

### Sublime Text 3

Sublime installation guide [link](https://www.sublimetext.com/docs/3/linux_repositories.html#apt)

```
$ wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
$ sudo apt-get install apt-transport-https
$ echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
$ sudo apt-get update
$ sudo apt-get install sublime-text
```

### VirtualBox v5.0.40

```
$ sudo apt-get install virtualbox
```

### PhpStorm 2017.3

[Download](https://download-cf.jetbrains.com/webide/PhpStorm-2017.3.4.tar.gz)

```
$ tar -xvf PhpStorm-2017.3.4.tar.gz
$ mv PhpStorm-173.4548.32/ phpstorm/
$ cd phpstorm/bin
$ ./phpstorm
```

### Eclipse Oxygen v2

[Download](http://www.eclipse.org/downloads/download.php?file=/technology/epp/downloads/release/oxygen/2/eclipse-jee-oxygen-2-linux-gtk-x86_64.tar.gz)

```
$ tar -xvf eclipse-jee-oxygen-2-linux-gtk-x86_64.tar.gz
$ cd eclipse
$ ./eclipse
```


## Authors

* **Crysthoffer Amira Ratier** - *Initial work* - ![Linkedin](https://www.linkedin.com/in/crysthofferatier/)