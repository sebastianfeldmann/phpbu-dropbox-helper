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

## Install & Usage

### Clone

    git clone git@github.com:sebastianfeldmann/phpbu-dropbox-helper.git
    cd phpbu-dropbox-helper
    composer install
    bin/dropbox

### Composer

    composer install phpbu/phpbu-dropbox-helper
    vendor/bin/dropbox
