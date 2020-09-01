# htaccess
#Increase Security with X-Security Header - htaccess


  Header unset X-Powered-By
  Header set Content-Security-Policy "connect-src 'self';"
  Header always set Referrer-Policy "same-origin"
  Header always set X-Frame-Options "SAMEORIGIN"
  Header always set X-Xss-Protection "1; mode=block"
  Header always set X-Content-Type-Options "nosniff"
  Header always set Feature-Policy "microphone 'none'; payment 'none'; sync-xhr 'self' https://site.com"
  Header always set Strict-Transport-Security "max-age=63072000; includeSubDomains"
  Header set Public-Key-Pins "pin-sha256=\"base64+primary==\"; pin-sha256=\"base64+backup==\"; max-age=5184000; includeSubDomains"
  Header always set X-Permitted-Cross-Domain-Policies: "master-only"
