## requirements

docker

wskdeploy

node

wsk

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

1. include `-i` flag each time you run `wsk` commands against local env

2. you need to setup additional key in config - don't ask me why ...

```
APIGW_ACCESS_TOKEN=foo
```

therwise this happens:

```
Error: manifestreader.go [113]: [ERROR_YAML_FILE_FORMAT_ERROR]: File: [manifest.yml]: 
==> manifest_parser.go [1153]: [ERROR_WHISK_CLIENT_INVALID_CONFIG]: msg_config_missing_apigw_access_token
```

## wskprops

in case .wskprops failed to genrate you can always use guest auth from oficial repo:

`https://raw.githubusercontent.com/apache/incubator-openwhisk/master/ansible/files/auth.guest`

