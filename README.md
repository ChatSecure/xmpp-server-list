# xmpp-server-list
Public XMPP server list and metadata in JSON format. This list only includes servers with 'A' grade on [xmpp.net](https://xmpp.net) and that allow [In-Band Registration (XEP-0077)](https://xmpp.org/extensions/xep-0077.html).

Example:

```javascript
{
  "servers": [
    {
      "name": "Calyx Institute",
      "description": "Non-profit education and research organization focused on privacy technology.",
      "website": "https://www.calyxinstitute.org",
      "twitter": "https://twitter.com/calyxinstitute", // optional
      "privacy_policy": "https://www.calyxinstitute.org/legal/privacy-policy",
      "logo": "images/calyx.jpg", // can be relative path or absolute URL to an image
      "country_code": "NL",
      "domain": "jabber.calyxinstitute.org",
      "server": "jabber.calyxinstitute.org",
      "onion": "ijeeynrc6x2uy5ob.onion", // optional
      "port": 5222,
      "requires_otr": true, // indicates if server rejects non-OTR messages
      "captcha": false, // if server requires captcha for in-band registration
      "extensions": ["XEP-0163", "XEP-0065"], // Supported XEP extensions
      "certificate": "MIIFwzCCBKugAwIBAgIDAivsMA0GCSqGSIb3DQEBCwUAMEcxCzAJBgNVBAYTAlVTMRYwFAYDVQQKEw1HZW9UcnVzdCBJbmMuMSAwHgYDVQQDExdSYXBpZFNTTCBTSEEyNTYgQ0EgLSBHMzAeFw0xNTAyMDYwNDQzMDRaFw0xNjAzMTAwODIwMDZaMIGYMRMwEQYDVQQLEwpHVDcwMjc0Nzg2MTEwLwYDVQQLEyhTZWUgd3d3LnJhcGlkc3NsLmNvbS9yZXNvdXJjZXMvY3BzIChjKTE1MS8wLQYDVQQLEyZEb21haW4gQ29udHJvbCBWYWxpZGF0ZWQgLSBSYXBpZFNTTChSKTEdMBsGA1UEAwwUKi5jYWx5eGluc3RpdHV0ZS5vcmcwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQDCTdLiJ5/UTGjpAU9+pFY/gwYqdjZ5W045BXenSIkDqEkGqASgAmr76uIJgeIR2+gaySV4B1PBVRBwu4gOwOnry2skdfJdX/E3LPf2qz8+9T7aesvb684JHoInIH6OyUviG7/yclUKwyetz5hO/FO4KY1SP83Wb3Q9GCBRN8VWVC0P3MP8cySo+jXKOEPbCpbzKvsDRAzcyVpTUBHhnxRLuOcjNJREVnkWmAZdT8NW9qyNYTVPMaYZXcNGUAa9uSnR0AD5Vpqg5OW6VjVNh/veBdVg4+mQUVxtJoMLCzc4n3Ps73ZRITVPdpllB3w6jOhyLSzyIVRQj8q2jCb7xdkDGGInGyOOqxSC+E7Cuz5XlRf6DUFXQdlonegkzKrmTNhiLkMeNvVHxr8IFZCnmpBUdnBI8zn+GdBlXIkBTjYMoMzxayE+8UftF36nAXS8xWa/J5iBsNsETpdNT6upQ3vHzCvBK5TZAd4GQGK6ghdca5JbgwLWNZqLYnhhw4YxSNZxlle3sG5c/nzltp4StNXodR4qXcXlN4ay363zOYBgmDzyjlKph0fCPZwbCby+26w61pwXAgVJP+sLMu96ZsHNnfTZxUo3v3tsztMiU1WekXR1rO9fMAQ2bAHFB66OwRiIZgu1OtniQW+rPm7A1JD9d1/IO4LFkgqWQxCmpPsZrwIDAQABo4IBZDCCAWAwHwYDVR0jBBgwFoAUw5zz/NNGCDS7zkZ/oHxb8+IIy1kwVwYIKwYBBQUHAQEESzBJMB8GCCsGAQUFBzABhhNodHRwOi8vZ3Yuc3ltY2QuY29tMCYGCCsGAQUFBzAChhpodHRwOi8vZ3Yuc3ltY2IuY29tL2d2LmNydDAOBgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwEGCCsGAQUFBwMCMDMGA1UdEQQsMCqCFCouY2FseXhpbnN0aXR1dGUub3JnghJjYWx5eGluc3RpdHV0ZS5vcmcwKwYDVR0fBCQwIjAgoB6gHIYaaHR0cDovL2d2LnN5bWNiLmNvbS9ndi5jcmwwDAYDVR0TAQH/BAIwADBFBgNVHSAEPjA8MDoGCmCGSAGG+EUBBzYwLDAqBggrBgEFBQcCARYeaHR0cHM6Ly93d3cucmFwaWRzc2wuY29tL2xlZ2FsMA0GCSqGSIb3DQEBCwUAA4IBAQCKbCIimuh3jSQCxZw5n8oHMbJxZoBvbo8awn3N6d7LZ4CF/LJhCyOJilDY1pyjKKCq8vz5haYJWw1dUiMiVlZ/mubmYvnSZ4rvpOV37HxUQXfujowHTQWBOhNiEFzI+/EwZgKmUxW9WwNLpTAOqfebN85RuWUq5EAvFZ3iEaYxnMevbZVOvg32GuqLWfLfTiFX/aeTeKsuG2O08xzqLX+tpHDU6MiNM6TFELd2xwB31xW9KhZqrzSq27PUT/lWrS4teQvbLFWcytORaim55sTw77Y5z/BuMbvBDxZYThzxIZNd9WDw1odck1llbuUe15NKMRpCfjWgwZ2K/W6K73ve"
    }
  ]
}
```

## Domain and Server

Some servers have a domain of `example.com` and a server of `xmpp.example.com`. Server should be the result of SRV lookup, you can retrieve it with dig: `dig _xmpp-client._tcp.example.com SRV`.

This is here mainly to make it possible for users to connect via Tor to servers without .onions, because SRV lookups are not possible over Tor.

## Logos

Logos should have a 1:1 aspect ratio.

## Extensions

You only need to include info about XEP-0357 and XEP-0363. You can omit other extensions, these are the only two required for clients to work properly.

## Certificates

For the `certificate` key we need the certificate in 'der' format, converted to base64 with no linebreaks.

You can get the certificate in PEM format from the result on xmpp.net, which needs to be converted:

    $ openssl x509 -outform der -in certificate.pem | openssl enc -base64 -A -out certificate.cer.base64

Or you can get it directly from the XMPP server:

    $ openssl s_client -starttls xmpp -showcerts -connect <server.address>:5222 < /dev/null 2>/dev/null | openssl x509 -outform der | openssl enc -base64 -A -out certificate.cer.base64

Option `-starttls xmpp` should only be used for servers using STARTTLS. When in doubt try with and without it.
