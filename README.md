# slopcannon-react-spa
## React SPA

Basic Vite + React single page app, built into a container image with [Cloud Native Buildpacks](https://buildpacks.io/) (Paketo Node.js buildpack with nginx web server).

Local dev: `npm install && npm run dev`

Build image (requires `pack` and Docker):

    pack build slopcannon-react-spa --builder paketobuildpacks/builder-jammy-base

Settings come from `project.toml`. Run: `docker run -p 8080:8080 slopcannon-react-spa`
