# Actions

Favorite GitHub Actions.

## Dokku

Deploys the code using `dokku`. How to setup:

1. Add the following secrets in `https://github.com/<user>/<repo>/settings/secrets`:

   - `DOKKU_USER`: User on the server running `dokku`
   - `DOKKU_HOST`: IP host of the server
   - `DOKKU_APP`: Name of the app in `dokku`
   - `DOKKU_PORT`: Port used by `ssh`, tends to be `22`
   - `BRANCH_FROM`: Branch to deploy from your repo
   - `BRANCH_TO`: Branch to deploy set in `dokku`
   - `PRIVATE_KEY`: User private key (no passphrase)
   - `PUBLIC_KEY`: User public key (no passphrase)

2. Commit `.github/workflows/dokku.yml` into your project

3. Now the action will deploy your project automatically.
