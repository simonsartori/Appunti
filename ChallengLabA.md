### setting directories
$ sudo mkdir /directory1
$ sudo mkdir /directory2
$ sudo mkdir /directory3

### setting groups
$ sudo groupadd dipartimento1
$ sudo groupadd dipartimento2
$ sudo groupadd dipartimento3

### adding admin of department
$ sudo ureradd admin_dipartimento1
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
$ sudo useradd employerA
$ sudo useradd employerB

### setting passowrd of emplyers
$ sudo passwd employerA
$ sudo passwd employerB