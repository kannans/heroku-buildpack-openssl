# heroku-buildpack-openssl
Buildpack for OpenSSL 1.1.1t on Heroku

This downloads, builds and installs OpenSSL 1.1.1t, installing at
/app/

We have to export and link the etc/ssl folder.

 ```
 export LD_LIBRARY_PATH=/app/openssl/lib/
 ln -s /etc/ssl /app/openssl/ssl 
```

