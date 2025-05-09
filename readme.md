# Abstract

Components extracted from serverOS repo. Automatically renews TLS certificate when enabled.

Reverse proxy all traffic to *:80/.well-known/acme-challenge at `http://unix:/run/serverOS-certauto/certauto.sock`, adapt config and services file, set `Wants` dependency on serverOS-TLS-holder in your reverse proxy config.
