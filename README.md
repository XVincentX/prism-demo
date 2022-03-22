# Prism Demo

1. Run the conversion tool to get an OpenAPI file from the CSDL one

`npx odata-openapi3 ./schema.csdl`

2. Run Prism on the generated document and the flag you would like to see:

`npm exec @stoplight/prism-cli mock schema.openapi3.json -- --dynamic --multiprocess`

3. Enjoy the mock server