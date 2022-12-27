---
title: documentation
---


<p align="center"><img src="assets/stack.svg"></p>

## vector tile generator

- [x] done with [tilemaker](https://tilemaker.org)
- [ ] needs documentation
- [ ] migrate to [shortbread]("https://shortbread.geofabrik.de) scheme

## image tile generator

- [ ] maybe summer 2023

## cloud converter

- [x] already works: [github.com/OpenCloudTiles/opencloudtiles-converter](https://github.com/OpenCloudTiles/opencloudtiles-converter)
- [x] implements the new [cloudtiles format](https://github.com/OpenCloudTiles/opencloudtiles-converter/blob/main/readme.md), similar to [PMTiles](https://github.com/protomaps/PMTiles)

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


<table style="width:100%">
	<tr>
		<td class="center">component</td>
		<td>status</td>
		<td>description</td>
	</tr>
	<tr>
		<td class="center">OSM</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">tile generator</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">*.mbtiles</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">tiles converter</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">*.cloudtiles</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">tiles server</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">CDN</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td class="center">frontend</td>
		<td></td>
		<td></td>
	</tr>
</table>