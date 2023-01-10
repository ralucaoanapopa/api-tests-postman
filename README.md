
# Setup

1. [Download](https://www.postman.com/downloads/) and install postman

2. Import collections from this repo

3. Download and install [node.js](https://nodejs.org/en/download/current/)

4. Install [newman](https://www.npmjs.com/package/newman) from cmd:

```
npm install -g newman
```

Decided to use [environment variables](https://learning.postman.com/docs/sending-requests/managing-environments/) because:
- global variables have lower precedence and can be overridden by environment variables
- seems more natural to use `--environment` option when [running collection using newman](https://github.com/postmanlabs/newman/#newman-run-collection-file-source-options)


# APIs used

## REST
- [BookCart API](https://bookcart.azurewebsites.net/swagger/index.html)
- [Library API](https://glitch.com/edit/#!/postman-library-api?path=README.md)

## SOAP
- [Numbers](https://www.dataaccess.com/webservicesserver/NumberConversion.wso)
- [Calculator](http://www.dneonline.com/calculator.asmx)
- [Country Info](http://webservices.oorsprong.org/websamples.countryinfo/CountryInfoService.wso)
- [Temperature](https://www.w3schools.com/xml/tempconvert.asmx)

# Tools

## Postman

Run collection with tests for BookCart API using Postman UI:

![](https://github.com/ralucaoanapopa/api-tests-postman/blob/main/BookCart_run_collection.gif)

## [Newman](https://learning.postman.com/docs/running-collections/using-newman-cli/command-line-integration-with-newman/)

### Run tests from a collection

```
newman run <collection_name.json> -e <environment_file.json>
```
Run collection with tests for Library API using newman

![](https://github.com/ralucaoanapopa/api-tests-postman/blob/main/LibraryAPI_run_newman.gif)

# Readings

- [REST API - IBM](https://www.ibm.com/topics/rest-apis)
- [REST API - RedHat](https://www.redhat.com/en/topics/api/what-is-a-rest-api)
- [SOAP vs REST - RedHat](https://www.redhat.com/en/topics/integration/whats-the-difference-between-soap-rest)
- [SOAP vs REST - SoapUI](https://www.soapui.org/learn/api/soap-vs-rest-api/)

