Use CloudFlare Worker for free deployment

Introduction
CloudFlare Worker is CloudFlare's edge computing service. Developers can program the CDN through JavaScript, so that they can handle HTTP requests flexibly. This allows many tasks to be completed on the CDN without the involvement of its own server.

deploy
Homepage: https://workers.cloudflare.com

Registration, login, Start building, take a subdomain name, Create a Worker.

Copy index.js to the code box on the left, Save and deploy. If it is normal, the home page should be displayed on the right.

The https://xxxx.subdomain.workers.dev in the favorite address box can be accessed directly in the future.

Billing
Go back to the overview page to see the usage. The free version has 100,000 free requests per day, which is usually sufficient for individuals.

If it is not enough, you can register multiple Workers and configure multi-line load balancing in conf.js. Or upgrade to the $5 premium version, which can be used for 10 million requests per month (exceeding $0.5/million requests).

Change setting
By default, static resources are reverse-proxy from https://etherdream.github.io/jsproxy, which can be configured through ASSET_URL in the code, so that a custom conf.js configuration can be used.

There is a problem
WebSocket proxy has not been implemented

External chain restrictions have not yet been implemented

Not fully tested, perfect later
