# HTTPS SSL scripts

Scripts for the HTTPS SSL project.

- `0-world_wide_web` - shows the DNS records of a domain's subdomains
  (`www`, `lb-01`, `web-01`, `web-02`) or of one specific subdomain.
- `1-haproxy_ssl_termination` - HAProxy config that terminates SSL on
  port 443 and serves the web servers over HTTPS.
- `2-redirect_http_to_https` - HAProxy config that also answers HTTP
  with a 301 redirect to HTTPS.

Usage:

    ./0-world_wide_web kpaul.tech
    ./0-world_wide_web kpaul.tech web-02
