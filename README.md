# Prism Demo

1. Install and run the conversion tool to get an OpenAPI file from the CSDL one

`dotnet tool restore`
`dotnet tool run hidi transform -cs schema.csdl -o openapi.yaml`

2. Run Prism on the generated document and the flag you would like to see:

`npm exec @stoplight/prism-cli mock openapi.yaml -- --dynamic --multiprocess`

3. Enjoy the mock server