# 0x10. HTTPS SSL

![ALT](https://github.com/islam-solaiman/alx-system_engineering-devops/blob/master/0x10-https_ssl/HTTPS.png?raw=true)

This Project is about importance of HTTPS and how it works and configration of HolbertonBnB web servers with certbot certificate and HAproxy SSL termination.

#TASKS:

## Task0: World wide web**
  * [1-world_wide_web](./0-world_wide_web): Bash script that displays
  information about subdomains on my configured servers.
  * Usage: `./1-world_wide_web <domain> <subdomain>`
  * Output: `The subdomain [SUB_DOMAIN] is a [RECORD_TYPE] record and
  points to [DESTINATION]`
  * If no `subdomain` parameter is passed, displays information about the
  subdomains `www`, `lb-01`, `web-01` and `web-02`, in that order.

## Task1: HAproxy SSL termination**
  * [2-haproxy_ssl_termination](./2-haproxy_ssl_termination): HAproxy
  configuration file that accepts encrypted SSL traffic for the subdomain
  `www.` on TCP port 443.

## Task2: No loophole in your website traffic**
