---
title: "Sign your Certs!"
date: 2022-11-23T14:20:28Z
draft: true
tags: ["programming"]
featured_image: "https://letsencrypt.org/images/letsencrypt-logo-horizontal.svg"
---

git config --global user.email yourgitemail@example.com

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install letsencrypt


````
certbot certonly \
    --manual \
    --preferred-challenges=dns \
    --email your@email-address.com \
    --agree-tos \
    --config-dir ./config \
    --logs-dir ./logs \
    --work-dir ./workdir \
    -d example.com
```

DNS settings

Private certificate (privkey.pem)
Public certificate (cert.pem)
Public certificate chain (fullchain.pem).