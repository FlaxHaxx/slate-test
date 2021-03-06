# Northbricks API Documentation

This is Northbricks website for developers.

The website contains both static content and content generated from the Swagger specificationsof the REST API. See [update swagger spec](#update-swagger-spec) to see how to update the generated content.

## Run local server

Install widdershins.
```sh
npm install -g widdershins
npm install widdershins
```

Start local server.
```sh
bundle exec middleman server
```

## Deploy

Deploy to production.
```sh
./deploy.sh
```

## Update swagger spec

Copy latest swagger files to `source/swagger/` and name them `[service-name].swagger.yaml`.

Generate documentation from swagger files with `widdershins`.
```sh
node node_modules/widdershins/widdershins.js -y -n -c -s -l source/swagger/transaction.swagger.yaml -o source/includes/_transaction.swagger.md
node node_modules/widdershins/widdershins.js -y -n -c -s -l source/swagger/user.swagger.yaml -o source/includes/_user.swagger.md
```

Now remove the first section in the generated file(s).