# Cloudflare metrics
Send your page views from Cloudflare worker to InfluxDB.

# My Dashboard views


![Screenshot 2023-02-04 184359](https://user-images.githubusercontent.com/93249038/216769959-f0260357-8004-4741-8ab0-ccb000906f27.png)

# Requirements
1) Your site need to be setup behind Cloudflare CDN.

2) You need to setup InfluxDB with external access (make sure you have set authentication)

3) Make sure InfluxDB is hosted under supported port for Workers. Best option is 80 or 443.

# How to use
1) Install wrangler package

"npm i @cloudflare/wrangler -g"

2) Copy example files

cp .env.example .env

cp wrangler.toml.example wrangler.toml

3) Deploy your worker to a site with wrangler

"wrangler publish --env production"

(Optional) If you're using Grafana with InfluxDB, then you can import example Dashboard from first screen.
