## requirements

docker

wskdeploy

node

## setup

```
npm run local-dev
```

open new terminal tab

```
npm run show-props
```

you can update your `~/.wskprops` or create new credentials file and use `--config` flag for `wskdeploy`

## deployment

npm run local-deploy

## known issues

you need to setup additional key in config - don't ask me why ...

```
APIGW_ACCESS_TOKEN=foo
```

therwise this happens:

```
Error: manifestreader.go [113]: [ERROR_YAML_FILE_FORMAT_ERROR]: File: [manifest.yml]: 
==> manifest_parser.go [1153]: [ERROR_WHISK_CLIENT_INVALID_CONFIG]: msg_config_missing_apigw_access_token
```
