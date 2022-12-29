---
title: Documentation
---

<style>
	.chart-block {
		text-align: center;
		width: 140px;
		position: relative;
	}
	.chart-block svg {
		position: absolute;
		top: 0px;
		left: 0px;
		height: 100%;
		width: 120px;
	}
	.chart {
		width:100%;
	}
	.chart td:first-child {
		text-align: center;
		vertical-align: middle;
		width:130px;
	}
	.chart td:last-child {
		border-top: 1px solid rgba(128,128,128,0.4);
	}
</style>

<svg>
	<symbol id="chart-block" viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice">
		<g transform="translate(0, 500)">
			<path d="M 60 -500 L 60 0" fill="none" stroke="#888" stroke-miterlimit="10" pointer-events="stroke"/>
			<path d="M 60 -1 L 63.5 -8 L 60 -6.25 L 56.5 -8 Z" fill="#888" stroke="#888" stroke-miterlimit="10" pointer-events="all"/>
			<path d="M 60 40 L 60 540" fill="none" stroke="#888" stroke-miterlimit="10" pointer-events="stroke"/>
			<rect x="1" y="0" width="118" height="40" style="fill:rgba(255,0,0,0.2);stroke:#844; stroke-width:1px" pointer-events="all" />
		</g>
	</symbol>
</svg>

<table class="chart">
<tr>
<td class="chart-block">
	<svg viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice" >
		<use xlink:href="#chart-block" style="filter: hue-rotate(80deg);" />
		<text x="60" y="520" text-anchor="middle" font-size="12">tile generator</text>
		<text x="60" y="525" text-anchor="middle" dominant-baseline="hanging" font-size="8">80%</text>
	</svg>
</td>
<td>

## vector tile generator

- [x] converts OSM to *.mbtiles, done with [tilemaker](https://tilemaker.org)
- [ ] needs documentation
- [ ] migrate to [shortbread]("https://shortbread.geofabrik.de) scheme

## image tile generator

Based on NASA, ESA on BKG (germany). Implemented sometime in 2023.

</td>
</tr>

<tr>
<td>
	*.mbtiles
</td>
<td>
Necessary intermediate format, but is not suitable for a scalable cloud server infrastructure.
</td>
</tr>

<tr>
<td class="chart-block">
	<svg viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice">
		<use xlink:href="#chart-block" style="filter: hue-rotate(100deg);" />
		<text x="60" y="520" text-anchor="middle" font-size="12">cloud tile converter</text>
		<text x="60" y="525" text-anchor="middle" dominant-baseline="hanging" font-size="8">100%</text>
	</svg>
</td>
<td>

## cloud tile converter

- [x] already works: [code](https://github.com/OpenCloudTiles/opencloudtiles-converter)

</td>
</tr>
<tr>
<td>*.cloudtiles</td>
<td>

implements the new [.cloudtiles format](https://github.com/OpenCloudTiles/opencloudtiles-converter/blob/main/readme.md), similar to [PMTiles](https://github.com/protomaps/PMTiles)

</td>
</tr>
<tr>
<td class="chart-block">
	<svg viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice">
		<use xlink:href="#chart-block" style="filter: hue-rotate(50deg);" />
		<text x="60" y="520" text-anchor="middle" font-size="12">cloud tile server</text>
		<text x="60" y="525" text-anchor="middle" dominant-baseline="hanging" font-size="8">50%</text>
	</svg>
</td>
<td>

## cloud server

- [ ] will be added to: [opencloudtiles-converter](https://github.com/OpenCloudTiles/opencloudtiles-converter)
- [ ] also a node.js implementation?
- [ ] A flexible CORS system to serve tiles, styles and glyphs under multiple domains.

</td>
</tr>
<tr>
<td class="chart-block">
	<svg viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice">
		<use xlink:href="#chart-block" style="filter: hue-rotate(50deg);" />
		<text x="60" y="520" text-anchor="middle" font-size="12">CDN</text>
		<text x="60" y="525" text-anchor="middle" dominant-baseline="hanging" font-size="8">50%</text>
	</svg>
</td>
<td>

## CDN

- [ ] add manuals and reference implementations for:
	- [ ] bunny.net
	- [ ] Google Cloud
	- [ ] Amazon
	- [ ] CloudFlare
- [ ] has to take care of:
	- [ ] CORS
	- [ ] precompression
	- [ ] styles+fonts

</td>
</tr>
<tr>
<td class="chart-block">
	<svg viewBox="0 0 120 1040" preserveAspectRatio="xMidYMid slice">
		<use xlink:href="#chart-block" style="filter: hue-rotate(80deg);" />
		<text x="60" y="520" text-anchor="middle" font-size="12">frontend</text>
		<text x="60" y="525" text-anchor="middle" dominant-baseline="hanging" font-size="8">80%</text>
	</svg>
</td>
<td>

## frontend

- based on [MapLibre](https://github.com/maplibre/maplibre-gl-js)
- add multiple shortbread styles

</td>
</tr>
<tr>
<td>User</td>
<td>

`sudo make user happy`

</td>
</tr>
</table>