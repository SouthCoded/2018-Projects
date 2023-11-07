After setup, your mailserver should be ready to send and receive mail. To receive mail, setup your mail client with the appropriate information.
Mainly setting the server to mail.{{ your domain }} and making sure that the firewall settings on your machine allow outside connections. To send 
emails an easy tool to use is sendemail. Below is an example request I made. 

```
sendemail -t <insert_email> -s mail.rabbit.cricket -m hello -f test@rabbit.cricket -xu test@rabbit.cricket -xp password -o tls=no

```

Where -t is the receiving email address, -s is the mail server, -m is the message, -f is the sender address, -xu is the mail user, -xp is the mail
password and -o signifies to ignore TLS errors. 
