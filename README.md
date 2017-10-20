# bae-test

[![License](https://img.shields.io/badge/license-AGPL%20v3-blue.svg?style=flat)](http://www.gnu.org/licenses/agpl.html) [![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](http://bae-test.readthedocs.io/en/latest/) [![Docker](https://img.shields.io/docker/pulls/fiware/bae-test.svg)](https://hub.docker.com/r/fiware/bae-test) [![Support](https://img.shields.io/badge/support-askbot-yellowgreen.svg)](https://ask.fiware.org)

 * [Introduction](#introduction)
 * [GEi Overall Description](#gei-overall-description)
 * [Installation](#build-and-install)
 * [API Overview](#api-overview)
 * [API Reference](#api-reference)
 * [Testing](#testing)
 * [Advanced Topics](#advanced-topics)

# Introducction

This is the main repository of the Business API Ecosystem. This project is part of [FIWARE](https://www.fiware.org), and has been developed in 
collaboration with the [TM Forum](https://www.tmforum.org/). Check also the [FIWARE Catalogue entry for the Business API Ecosystem](https://catalogue.fiware.org/enablers/bae-test-biz-ecosystem-ri)!

The Business API Ecosystem is not a single software repository, but it is composed of different projects which work coordinatelly to provide the complete functionality.

Concretely, the Business API Ecosystem is made of the following components:

* Reference implementations of TM Forum APIs.
    * [Catalog Management API](https://github.com/FIWARE-TMForum/DSPRODUCTCATALOG2)
    * [Product Ordering Management API](https://github.com/FIWARE-TMForum/DSPRODUCTORDERING)
    * [Product Inventory Management API](https://github.com/FIWARE-TMForum/DSPRODUCTINVENTORY)
    * [Party Management API](https://github.com/FIWARE-TMForum/DSPARTYMANAGEMENT)
    * [Customer Management API](https://github.com/FIWARE-TMForum/DSCUSTOMER)
    * [Billing Management API](https://github.com/FIWARE-TMForum/DSBILLINGMANAGEMENT)
    * [Usage Management API](https://github.com/FIWARE-TMForum/DSUSAGEMANAGEMENT)

* Rating, Charging, and Billing backend.
    * [Charging Backend](https://github.com/FIWARE-TMForum/bae-charging-backend-test)

* Revenue Settlement and Sharing System.
    * [RSS](https://github.com/FIWARE-TMForum/bae-rss-test)

* Authentication, API Orchestrator, and Web portal.
    * [Logic Proxy](https://github.com/FIWARE-TMForum/bae-logic-proxy-test)

Any feedback is highly welcome, including bugs, typos or things you think should be included but aren't. To provide feedback you can use the 
general [GitHub issues](https://github.com/FIWARE-TMForum/bae-test/issues/new), or provide it directly to the components using the [Charging Backend Issues](https://github.com/FIWARE-TMForum/bae-charging-backend-test/issues/new), [RSS Issues](https://github.com/FIWARE-TMForum/bae-rss-test/issues/new), or [Logic Proxy Issues](https://github.com/FIWARE-TMForum/bae-logic-proxy-test/issues/new).

# GEi Overall Description

The Business API Ecosystem is a joint component made up of the FIWARE Business Framework and a set of APIs (and its reference implementations) provided by the TMForum. This component allows the monetization of different kind of assets (both digital and physical) during the whole service life cycle, from offering creation to its charging, accounting and revenue settlement and sharing. The Business API Ecosystem exposes its complete functionality through TMForum standard APIs; concretely, it includes the catalog management, ordering management, inventory management, usage management, billing, customer, and party APIs.

# Installation

The instructions to install the Business API Ecosystem can be found at the [Installation Guide](http://bae-test.readthedocs.io/en/latest/installation-administration-guide.html). You can install the software in three different ways:

* Using the provided scripts
* Using a [Docker Container](https://hub.docker.com/r/fiware/bae-test)
* Manually

# API Overview

The Business API Ecosystem API is build up using the APIs of the different components each exposing its own resources.

## Catalog API

The Catalog API is available under /DSProductCatalog/api/ and its main resources are:

* Categories
* Catalogs
* Product Specifications
* Product Offerings

## Ordering API

The Ordering API is available under /DSProductOrdering/api/ and its main resources are:

* Product Order

## Inventory API

The Inventory API is available under /DSProductInventory/api/ and its main resources are:

* Product

## Party API

The Party API is available under /DSPartyManagement/api/ and its main resources are:

* Individual
* Organization

## Customer API

The Customer API is available under /DSCustomerManagement/api/ and its main resources are:

* Customer
* Customer Account

## Billing API

The Billing API is available under /DSBillingManagement/api/ and its main resources are:

* Billing Account
* Applied Billing Charge

## Usage API

The Usage API is available under /DSUsageManagement/api/ and its main resources are:

* Usage
* Usage Specification

## RSS API

The RSS API is available under /DSRevenueSharing/rss/ and its main resources are:

* Revenue Sharing Model
* Transaction
* Revenue Sharing Report

# API Reference

For further documentation, you can check the API Reference available at:

* [Apiary](http://docs.fiwaretmfbizecosystem.apiary.io) 
* [Github Pages](https://fiware-tmforum.github.io/bae-test/)

# Testing

## End-to-End tests

End-to-End tests are described in the [Installation Guide](http://bae-test.readthedocs.io/en/latest/installation-administration-guide.html#end-to-end-testing)

## Unit tests

The way of executing the unit tests is described in each of the components repositories

# Advanced Topics

* [User & Programmers Guide](doc/user-programmer-guide.rst)
* [Installation & Administration Guide](doc/installation-administration-guide.rst)

You can also find this documentation on [ReadTheDocs](http://bae-test.readthedocs.io)
