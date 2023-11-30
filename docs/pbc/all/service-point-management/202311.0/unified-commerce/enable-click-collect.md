---
title: Enable Click & Collect
description: Learn how to enable Click&Collect
last_updated: Nov 23, 2023
template: howto-guide-template
---

To enable the default implementation of Click & Collect, follow the steps.

## Prerequisites

Install the following features:

* [Service Points Cart + Checkout](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-cart-checkout-feature.html)
* [Service Points Cart](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-cart-feature.html)
* [Service Points + Customer Account Management](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-customer-account-management-feature.html)
* [Service Points](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-feature.html)
* [Service Points + Order Management](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-order-management-feature.html)
* [Service Points + Product Offer](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-product-offer-feature.html)
* [Service Points Cart + Shipment](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/install-features/install-the-service-points-shipment-feature.html)
* [Marketplace Merchant Portal Product Offer Service Points](/docs/pbc/all/offer-management/{{page.version}}/unified-commerce/install-features/install-the-marketplace-merchant-portal-product-offer-service-points-feature.html)
* [Marketplace Merchant + Product Offer Service Points Availability](/docs/pbc/all/offer-management/{{page.version}}/unified-commerce/install-features/install-the-marketplace-merchant-product-offer-service-points-availability-feature.html)
* [Marketplace Product Offer + Service Points](/docs/pbc/all/offer-management/{{page.version}}/unified-commerce/install-features/install-the-marketplace-product-offer-service-points-feature.html)
* [Product Offer Service Points Availability](/docs/pbc/all/offer-management/{{page.version}}/unified-commerce/install-features/install-the-product-offer-service-points-availability-feature.html)
* [Product Offer Service Points](/docs/pbc/all/offer-management/{{page.version}}/unified-commerce/install-features/install-the-product-offer-service-points-feature.html)
* [Shipment Cart](/docs/pbc/all/carrier-management/{{page.version}}/unified-commerce/install-features/install-the-shipment-cart-feature.html)
* [Shipment Product Offer Service Points Availability](/docs/pbc/all/carrier-management/{{page.version}}/unified-commerce/install-features/install-the-shipment-product-offer-service-points-availability-feature.html)
* [Shipment Service Points](/docs/pbc/all/carrier-management/{{page.version}}/unified-commerce/install-features/install-the-shipment-service-points-feature.html)
* [Install the Product Offer Shipment Availability feature](/docs/pbc/all/offer-management/{{page.version}}/marketplace/install-and-upgrade/install-features/install-the-product-offer-shipment-availability-feature.html)


## 1. Add service points and their addresses

To add service points and addresses using Glue API, see [Backend API Marketplace B2C Demo Shop reference](/docs/scos/dev/glue-api-guides/{{page.version}}/backend-glue-infrastructure/backend-api-marketplace-b2c-demo-shop-reference.html).

To import service points, see [Import file details: service_point.csv](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/import-and-export-data/import-file-details-service-point.csv.html).

To import service point addresses, see [Import file details: service_point_address.csv](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/import-and-export-data/import-file-details-service-point-address.csv.html).

## 2. Add service types

For Click & Collect, you most probably need the pickup service type.

To add service types using Glue API, see [Backend API Marketplace B2C Demo Shop reference](/docs/scos/dev/glue-api-guides/{{page.version}}/backend-glue-infrastructure/backend-api-marketplace-b2c-demo-shop-reference.html).

To import service types, see [Import file details: service_type.csv](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/import-and-export-data/import-file-details-service-type.csv.html).


## 3. Add services

You need to add services per service point based on the service types you've added.

To add services using Glue API, see [Backend API Marketplace B2C Demo Shop reference](/docs/scos/dev/glue-api-guides/{{page.version}}/backend-glue-infrastructure/backend-api-marketplace-b2c-demo-shop-reference.html).

To import service types, see [Import file details: service.csv](/docs/pbc/all/service-point-management/{{page.version}}/unified-commerce/import-and-export-data/import-file-details-service.csv.html).


## 4. Assign the service type to shipment type

To import service to shipment type assignments, see [Import file details: shipment_type_service_type.csv](/docs/pbc/all/carrier-management/{{page.version}}/base-shop/import-and-export-data/file-details-shipment-type-service-type.csv.html).


## 5. Assign product offers to shipment types

To import offers to shipment type assignments, see [Import file details: product_offer_shipment_type](/docs/pbc/all/offer-management/{{page.version}}/marketplace/import-and-export-data/import-file-details-product-offer-shipment-type.csv.html).