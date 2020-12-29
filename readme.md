# Actions

Favorite GitHub Actions.

## Dokku

Deploys the code using `dokku`. How to setup:

1. Add the following secrets in `https://github.com/<user>/<repo>/settings/secrets`:

   - `DOKKU_APP`: Name of the app in `dokku`
   - `DOKKU_HOST`: IP host of your server
   - `DOKKU_PORT`: Port used by `ssh`, usually `22`
   - `DOKKU_USER`: User on the server running `dokku`
   - `PRIVATE_KEY`: User private key (no passphrase)
   - `PUBLIC_KEY`: User public key (no passphrase)

2. Commit `.github/workflows/dokku.yml` into your project

3. Make a change to see the app deployed.

**Note:** Assumes your default branches are `main`
