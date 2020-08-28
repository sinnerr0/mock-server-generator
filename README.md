# Mock Server Generator

## Motivation

Open API를 사용하는 것이 아니라면 서버쪽과 클라이언트쪽이 동시에 개발이 진행 된다. 이런 경우 클라이언트쪽에 부담이 커지는데 API 스펙을 미리 확인했다고 하더라도 서버가 아직 없으므로(있더라도 일부만) 클라이언트쪽 작업이 지연되거나 Mocking을 해서 반환값을 가정하에 두고 개발을 해야 한다는 점이다. 서버쪽에서 협의된 API 스펙에 맞추어 서버에서 Mock서버를 구현해 준다면 상황이 좀 나아질테지만 개발하기도 바쁜데 이런걸 구현하는 것 자체가 쉽지 않다.

## Summary

서버와는 관계없이 정의된 인터페이스에 따라 미리 개발을 진행할 수 있도록 Mock Server를 생성하고 자동으로 생성된 응답값을 돌려준다.

## Base knowledge

Open API Spec 3.0.3 https://swagger.io/specification/

## Open API Spec File

- openapi.yaml

- Prism mock: Dynamic Response Generation

  https://meta.stoplight.io/docs/prism/docs/guides/01-mocking.md#dynamic-response-generation

## Create/Edit file

https://editor.swagger.io/

## Install

```
$ npm install
```

## Spin up a mock HTTP server

```
$ npm start
```

## Proxy Real Server

```
# Modify real server address in package.json
$ npm run proxy
```

## Docs UI

```
# serve port 4000: http://localhost:4000
$ npm run docs
```
