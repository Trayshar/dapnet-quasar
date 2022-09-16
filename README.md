# Dapnet App (dapnet-quasar)

New multi-platform frontend for [DAPNET v2](https://github.com/dapnet-core)

## Getting started
### Using docker
Run
```bash
docker build -t dapnet-quasar:latest . && docker run -p 80:80 dapnet-quasar:latest
```
and open a webbrowser at [localhost](http://localhost). This will launch the production build.

### Manually

Install node.js (≥ 18) and npm (or any other package manager) and install the dependencies
```bash
npm install
```

After that you can launch the development profile with
```bash
npm run dev
```

There is no backend connection at the moment. I will add a docker-compose file to allow easy deployment once that is set up.

## Why this rework?
There already is a working [web frontend for DAPNET v2](https://github.com/dapnet-core/web/tree/vuetify), but its using lots of outdated dependencies and is hard to migrate and maintain. Additionally, it only covers the web; DAPNET v1 has apps for [Android](https://github.com/DecentralizedAmateurPagingNetwork/DAPNETApp) and [iOS](https://apps.apple.com/ca/app/dapnet/id1638627303), which DAPNET v2 should match.

This project uses [Quasar Framework](https://quasar.dev/introduction-to-quasar), which can deploy to both the web and mobile devices.
