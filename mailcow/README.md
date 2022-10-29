# MailCow

is a mail system that has been dockerized to be 

## Overview
The integrated mailcow UI allows administrative work on your mail server instance as well as separated domain administrator and mailbox user access:

- DKIM and ARC support
- Black- and whitelists per domain and per user
- Spam score management per-user (reject spam, mark spam, greylist)
- Allow mailbox users to create temporary spam aliases
- Prepend mail tags to subject or move mail to sub folder (per-user)
- Allow mailbox users to toggle incoming and outgoing TLS enforcement
- Allow users to reset SOGo ActiveSync device caches
- imapsync to migrate or pull remote mailboxes regularly
- TFA: Yubikey OTP and U2F USB (Google Chrome and derivatives only), TOTP
- Add domains, mailboxes, aliases, domain aliases and SOGo resources
- Add whitelisted hosts to forward mail to mailcow
- Fail2ban-like integration
- Quarantine system
- Antivirus scanning incl. macro scanning in office documents
- Integrated basic monitoring
- A lot more...

mailcow: dockerized comes with multiple containers linked in one bridged network. Each container represents a single application.

- ACME
- ClamAV (optional)
- Dovecot
- MariaDB
- Memcached
- Netfilter (Fail2ban-like integration by @mkuron)
- Nginx
- Oletools via Olefy
- PHP
- Postfix
- Redis
- Rspamd
- SOGo
- Solr (optional)
- Unbound
- A Watchdog to provide basic monitoring

## More information about MailCow
- more about [MailCow](https://docs.mailcow.email/)
- Dockerized MailCow is saved at [Github](https://github.com/mailcow/mailcow-dockerized)
