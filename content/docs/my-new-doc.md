+++
title = "My New Doc"
description = "A sample doc"
date = 2018-05-16T13:15:24-06:00
weight = 20
draft = false
bref = "some descriptive text"
toc = true
+++

# My New Doc


This is some descriptive text.


Step | Task 
-----|-------
1.   | Underpants 
1.   | ???   
1.   | Profit 


1. Task 1

   ```bash
   some code
   ```
1. Task 2

  - subtask 1
  - subtask 2

1. Task 3


## Section 1

`some code`

```bash
$ some code here
echo some code
```

```css
code {
  padding: 2px;
  font-size: 85%;
  color: #FFFFFF;
  background-color: #757677;
  border-radius: 2px;
}
```

note

This is a test note

- 1
- 2


## This is a large image

![image 1](http://clouddocs.f5.com/containers/v2/_images/container_connectors_north-south.png)



### This is a wide code block table
```javascript
  {
   "class": "ADC",
   "schemaVersion": "0.0.1",
   "id": "urn:uuid:5cff92e8-d3d3-4056-8577-b0b170f812eb",
   "label": "Sample 2",
   "remark": "HTTPS with predictive-node pool",
   "updateMode": "selective",
   "Sample_02": {
     "class": "Tenant",
     "A1": {
       "class": "Application",
       "applicationType": "https",
       "vsMain": {
         "class": "VS_HTTPS",
         "virtualAddresses": [
           "10.0.2.10"
         ],
         "pool": "web_pool",
         "serverTLS": "webtls"
       },
       "web_pool": {
         "class": "Pool",
         "loadBalancingMode": "predictive-node",
         "monitors": [
           "http"
         ],
         "members": [
           {
             "servicePort": 80,
             "serverAddresses": [
               "192.0.2.10",
               "192.0.2.11"
             ]
           }
         ]
       },
       "webtls": {
         "class": "TLS_Server",
         "certificates": [
           {
             "certificate": "webcert"
           }
         ]
       },
       "webcert": {
         "class": "Certificate",
         "certificate": "-----BEGIN CERTIFICATE-----\nMIICnDCCAgWgAwIBAgIJAJ5n2b0OCEjwMA0GCSqGSIb3DQEBCwUAMGcxCzAJBgNVBAYTAlVTMRMwEQYDVQQIDApXYXNoaW5ndG9uMRAwDgYDVQQHDAdTZWF0dGxlMRQwEgYDVQQKDAtmNV9OZXR3b3JrczEbMBkGA1UEAwwSc2FtcGxlLmV4YW1wbGUubmV0MB4XDTE3MTEyNjE5NTAyNFoXDTE4MDIyNTE5NTAyNFowZzELMAkGA1UEBhMCVVMxEzARBgNVBAgMCldhc2hpbmd0b24xEDAOBgNVBAcMB1NlYXR0bGUxFDASBgNVBAoMC2Y1X05ldHdvcmtzMRswGQYDVQQDDBJzYW1wbGUuZXhhbXBsZS5uZXQwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBALEsuXmSXVQpYjrZPW+WiTBjn491mwZYT7Q92V1HlSBtM6WdWlK1aZN5sovfKtOX7Yrm8xa+e4o/zJ2QYLyyv5O+t2EGN/4qUEjEAPY9mwJdfzRQy6Hyzm84J0QkTuUJ/EjNuPji3D0QJRALUTzu1UqqDCEtiN9OGyXEkh7uvb7BAgMBAAGjUDBOMB0GA1UdDgQWBBSVHPNrGWrjWyZvckQxFYWO59FRFjAfBgNVHSMEGDAWgBSVHPNrGWrjWyZvckQxFYWO59FRFjAMBgNVHRMEBTADAQH/MA0GCSqGSIb3DQEBCwUAA4GBAJeJ9SEckEwPhkXOm+IuqfbUS/RcziifBCTmVyE+Fa/j9pKSYTgiEBNdbJeBEa+gPMlQtbV7Y2dy8TKx/8axVBHiXC5geDML7caxOrAyHYBpnx690xJTh5OIORBBM/a/NvaR+P3CoVebr/NPRh9oRNxnntnqvqD7SW0U3ZPe3tJc\n-----END CERTIFICATE-----",
         "privateKey": "-----BEGIN RSA PRIVATE KEY-----\nMIICXAIBAAKBgQCxLLl5kl1UKWI62T1vlokwY5+PdZsGWE+0PdldR5UgbTOlnVpStWmTebKL3yrTl+2K5vMWvnuKP8ydkGC8sr+TvrdhBjf+KlBIxAD2PZsCXX80UMuh8s5vOCdEJE7lCfxIzbj44tw9ECUQC1E87tVKqgwhLYjfThslxJIe7r2+wQIDAQABAoGAahUlWK1SRDojHqlEJ7QyoE6GExePotTtpDYEF93sZGX+LoNwuWT1ud98EFOnCNpG2Iw/sLaMsdJRaWYxBcrg+U6ER+Toi1lyQ9DgRk/KSaZHy6msSCCXtlSlBpbBcs9Aoy99tXLfPiKnKydQpBufh2N+RFFKFhIkhGGBJYkEY6ECQQDW6ASwVyg+mCSfSvenMCLKqRVTu7Qax7sdQa0fiowHeKvosRYkznFTywKmlyEeGWxAElkpbEXTR6efh+bkV3dzAkEA0w2wGGTGQBOZSwuKuMFzKvcyp7qwOdWZJVAyQ5sAb5/VKAn+S7k9IsT0ggiv2vCQDfol3An4plZLbWTHFXOb+wJAT8nc08vIOVUrY6jlwcDxaeTU8j2iZL77DaWwrSE3VB7NVJtK6WdsU/vvhAJgXVh7BF7Lk8GLOyJDbct7QhPnWQJBAMT/HcNnLPVaVdeKam2Rg+Iy4oFU7HDPQydk98XKxFlsoxXAXjBoMvxlQqStXxfJO20QdI4ycHkySy1Mx9bqFkkCQAZeNlQhmnFCcotpfHVzdwS5wgu3mDsG2nF3KhO2rYK+cnSE+bZaXw+GAF4pcPo2CAotdY/IJc/qYt7w2MLwYso=\n-----END RSA PRIVATE KEY-----",
         "passphrase": {
           "ciphertext": "ZjU=",
           "protected": "eyJhbGciOiJkaXIiLCJlbmMiOiJub25lIn0"
         }
       }
     }
   }
  }
```