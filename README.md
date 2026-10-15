# matthew5523.github.io

Holds one file that matters: `.well-known/appspecific/com.tesla.3p.public-key.pem`, the PUBLIC half of the key Home
Assistant uses to send charging commands to the car. Tesla reads it from
`https://matthew5523.github.io/.well-known/appspecific/com.tesla.3p.public-key.pem` when the app is registered.

A public key is safe to publish by design: it can only check signatures, never make them. The private half stays inside
Home Assistant. `.nojekyll` makes GitHub Pages serve the `.well-known` folder as plain files.
