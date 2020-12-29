# Actions

Favorite GitHub Actions.

### Dokku

Deploys the code using `dokku`. How to setup:

1. Add the following secrets in `https://github.com/<user>/<repo>/settings/secrets`:

   - `USER`: Dokku use on the server
   - `HOST`: IP host of the server
   - `APP`: Name of the app in dokku
   - `PORT`: Port used by `ssh`, tends to be 22
   - `FROM`: Branch to deploy from your repo
   - `TO`: Deploy branch used by dokku
   - `PUBLIC_KEY`: Dokku user public key (no passphrase)
   - `PRIVATE_KEY`: Dokku user private key (no passphrase)

2. Commit `.github/workflows/dokku.yml` into your project

3. Now the action will deploy your project automatically.
