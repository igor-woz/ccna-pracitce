
## Basic Router Security Part 1

This lab required me to: connect R1 and R2 together via their g0/0 interface, config appropriate hostnames, protect priv exec mode with a password, and verify how it is displayed in the running config.

To connect the routers I used a crossover cable, which is suitable for connecting devices of the same type, because they have the same TX/RX pin layout.

Hostname was configured using: `(config)#hostname <name>` command in the global config mode on each router. 

Password was configured using: `(config)#enable password cisco` command on each router. 

By default the above command stores the password as palintext, hence need for encryption. It is achieved by issuing: `(config)#service password-encryption` command, which now dispplays the passwords as type 7 encrypted strings. It is important to note that this type of enc. is weak and can be easily brute-forced.

Disabling the encryption by: `(config)#no service encryption` disables it for all next passwords, but does not decrypt already existind onees.

This concludes the 1st lab of the bunch.
