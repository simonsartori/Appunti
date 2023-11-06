### setting directories
$ sudo mkdir /Engeniring
$ sudo mkdir /Sales
$ sudo mkdir /IS

### setting groups
$ sudo groupadd dipartimento1
$ sudo groupadd dipartimento2
$ sudo groupadd dipartimento3

### adding admin of department
$ sudo useradd admin_dipartimento1
$ sudo ureradd admin_dipartimento2
$ sudo ureradd admin_dipartimento3

### setting password of the group admins
$ sudo passwd admin_dipartimentoA
$ sudo passwd admin_dipartimentoB
$ sudo passwd admin_dipartimentoC

### setting admin rights to admin accounts
$ sudo usermod -aG sudo admin_dipartimentoA
$ sudo usermod -aG sudo admin_dipartimentoB
$ sudo usermod -aG sudo admin_dipartimentoC

### setting employers
$ sudo useradd Marino
$ sudo useradd Simon

### setting passowrd of emplyers
$ sudo passwd Martino
$ sudo passwd Simon