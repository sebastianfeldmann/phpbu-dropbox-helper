# phpbu Dropbox Helper

Small script to obtain the "offline" refresh token that is
required for the phpbu Dropbox config.

```xml
<sync type="dropbox">
  <option name="refreshToken" value="MY_REFRESH_TOKEN" />
  <option name="appKey" value="APP_KEY" />
  <option name="appSecret" value="APP_SECRET" />
  <option name="path" value="/phpbu-backup/%Y" />
</sync>
```

For this script to work you have to create a Dropbox App in
your Dropbox App Center to obtain the `AppKey` and the `AppSecret`.

You will need both to obtain the necessary refresh token.

Run the script enter both, then you have to open a given URL in your browser and login with your Dropbox account.
This will authorize the app to access your account. You will receive an `AppCode`.
Enter this code on the prompt of the script to finally get your `RefreshToken`.

## Install & Usage

### Clone

    git clone git@github.com:sebastianfeldmann/phpbu-dropbox-helper.git
    cd phpbu-dropbox-helper
    composer install
    bin/dropbox

### Composer

    composer require --dev phpbu/phpbu-dropbox-helper
    vendor/bin/dropbox
