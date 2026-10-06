# MTA-STS policy for securitysolution.tech

Serves the [MTA-STS](https://datatracker.ietf.org/doc/html/rfc8461) policy at
<https://mta-sts.securitysolution.tech/.well-known/mta-sts.txt>, which tells sending mail servers to deliver
email to securitysolution.tech only over verified, encrypted connections.

The policy is in `testing` mode while TLS reports (TLS-RPT) are collected. Change `mode` to `enforce` once the
reports show clean delivery, then update the `id` in the `_mta-sts` DNS TXT record.
