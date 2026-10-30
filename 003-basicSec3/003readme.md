
## Basic Router Security Part 3

This lab goes over configuration from PC via a console port.

I changed the hostname to  R1, set  `enable secret cisco` to protect priv exec mode, and `enable password ccna` on the console line. 

Finally, I enabled login on the port via `R1(config-line)# login` command, and enabled encryption by running `service password-enc` command.

I verified all changes and saved the config.

