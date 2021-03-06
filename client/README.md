# Go API client for openapi

OFAC (Office of Foreign Assets Control) API is designed to facilitate the enforcement of US government economic sanctions programs required by federal law. This project implements a modern REST HTTP API for companies and organizations to obey federal law and use OFAC data in their applications.

## Overview
This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project.  By using the [OpenAPI-spec](https://www.openapis.org/) from a remote server, you can easily generate an API client.

- API version: v1
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.GoClientCodegen
For more information, please visit [https://github.com/moov-io/ofac](https://github.com/moov-io/ofac)

## Installation

Install the following dependencies:

```shell
go get github.com/stretchr/testify/assert
go get golang.org/x/oauth2
go get golang.org/x/net/context
go get github.com/antihax/optional
```

Put the package under your project folder and add the following in import:

```golang
import "./openapi"
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8084*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*OFACApi* | [**AddCompanyNameWatch**](docs/OFACApi.md#addcompanynamewatch) | **Post** /companies/watch | Add company watch by name. The match percentage will be included in the webhook&#39;s JSON payload.
*OFACApi* | [**AddCompanyWatch**](docs/OFACApi.md#addcompanywatch) | **Post** /companies/{companyId}/watch | Add OFAC watch on a Company
*OFACApi* | [**AddCustomerNameWatch**](docs/OFACApi.md#addcustomernamewatch) | **Post** /customers/watch | Add customer watch by name. The match percentage will be included in the webhook&#39;s JSON payload.
*OFACApi* | [**AddCustomerWatch**](docs/OFACApi.md#addcustomerwatch) | **Post** /customers/{customerId}/watch | Add OFAC watch on a Customer
*OFACApi* | [**GetCompany**](docs/OFACApi.md#getcompany) | **Get** /companies/{companyId} | Get information about a company, trust or organization such as addresses, alternate names, and remarks.
*OFACApi* | [**GetCustomer**](docs/OFACApi.md#getcustomer) | **Get** /customers/{customerId} | Get information about a customer, addresses, alternate names, and their SDN metadata.
*OFACApi* | [**GetLatestDownloads**](docs/OFACApi.md#getlatestdownloads) | **Get** /downloads | Return list of recent downloads of OFAC data
*OFACApi* | [**GetSDN**](docs/OFACApi.md#getsdn) | **Get** /sdn/{sdnId} | Specially designated national
*OFACApi* | [**GetSDNAddresses**](docs/OFACApi.md#getsdnaddresses) | **Get** /sdn/{sdnId}/addresses | Get addresses for a given SDN
*OFACApi* | [**GetSDNAltNames**](docs/OFACApi.md#getsdnaltnames) | **Get** /sdn/{sdnId}/alts | Get alternate names for a given SDN
*OFACApi* | [**Ping**](docs/OFACApi.md#ping) | **Get** /ping | Ping the OFAC service to check if running
*OFACApi* | [**RemoveCompanyNameWatch**](docs/OFACApi.md#removecompanynamewatch) | **Delete** /companies/watch/{watchId} | Remove a Company name watch
*OFACApi* | [**RemoveCompanyWatch**](docs/OFACApi.md#removecompanywatch) | **Delete** /companies/{companyId}/watch/{watchId} | Remove company watch
*OFACApi* | [**RemoveCustomerNameWatch**](docs/OFACApi.md#removecustomernamewatch) | **Delete** /customers/watch/{watchId} | Remove a Customer name watch
*OFACApi* | [**RemoveCustomerWatch**](docs/OFACApi.md#removecustomerwatch) | **Delete** /customers/{customerId}/watch/{watchId} | Remove customer watch
*OFACApi* | [**Search**](docs/OFACApi.md#search) | **Get** /search | Search SDN names and metadata
*OFACApi* | [**UpdateCompanyStatus**](docs/OFACApi.md#updatecompanystatus) | **Put** /companies/{companyId} | Update a Companies sanction status to always block or always allow transactions.
*OFACApi* | [**UpdateCustomerStatus**](docs/OFACApi.md#updatecustomerstatus) | **Put** /customers/{customerId} | Update a Customer&#39;s sanction status to always block or always allow transactions.


## Documentation For Models

 - [Address](docs/Address.md)
 - [Alt](docs/Alt.md)
 - [Download](docs/Download.md)
 - [OfacCompany](docs/OfacCompany.md)
 - [OfacCompanyStatus](docs/OfacCompanyStatus.md)
 - [OfacCustomer](docs/OfacCustomer.md)
 - [OfacCustomerStatus](docs/OfacCustomerStatus.md)
 - [Sdn](docs/Sdn.md)
 - [Search](docs/Search.md)
 - [UpdateCompanyStatus](docs/UpdateCompanyStatus.md)
 - [UpdateCustomerStatus](docs/UpdateCustomerStatus.md)
 - [Watch](docs/Watch.md)
 - [WatchRequest](docs/WatchRequest.md)


## Documentation For Authorization

 Endpoints do not require authorization.


## Author



