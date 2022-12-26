# OpenCloudTiles

powered by the community™

# Stack

<p align="center"><img src="assets/stack.svg?raw=true"></p>

## vector tile generator

- [x] done with [tilemaker](https://tilemaker.org)
- [ ] needs documentation
- [ ] migrate to [shortbread]("https://shortbread.geofabrik.de) scheme

## image tile generator

- [ ] maybe summer 2023

## cloud converter

- [x] works: [github.com/OpenCloudTiles/opencloudtiles-converter](https://github.com/OpenCloudTiles/opencloudtiles-converter)
- [x] implements a [cloudtiles format](https://github.com/OpenCloudTiles/opencloudtiles-converter/blob/main/readme.md), similar to [PMTiles](https://github.com/protomaps/PMTiles)

## cloud server

- [ ] will be added to: [github.com/OpenCloudTiles/opencloudtiles-converter](https://github.com/OpenCloudTiles/opencloudtiles-converter)
- [ ] also a node.js implementation?
- [ ] implement CORS

## CDN

- [ ] add manuals for:
  - [ ] bunny.net
  - [ ] Google Cloud
  - [ ] Amazon
  - [ ] CloudFlare
- [ ] has to take care of:
  - [ ] CORS
  - [ ] precompression
  - [ ] styles+fonts

## frontend

- based on [MapLibre](https://github.com/maplibre/maplibre-gl-js)
- add multiple shortbread styles
