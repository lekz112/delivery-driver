# openapi
No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This Dart package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: v0
- Build package: org.openapitools.codegen.languages.DartDioClientCodegen

## Requirements

Dart 1.20.0 or later OR Flutter 0.0.20 or later

## Installation & Usage

### Github
If this Dart package is published to Github, please include the following in pubspec.yaml
```
name: openapi
version: 1.0.0
description: OpenAPI API client
dependencies:
  openapi:
    git: https://github.com/GIT_USER_ID/GIT_REPO_ID.git
      version: 'any'
```

### Local
To use the package in your local drive, please include the following in pubspec.yaml
```
dependencies:
  openapi:
    path: /path/to/openapi
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```dart
import 'package:openapi/api.dart';


var api_instance = new BasketApi();
var addItemToBasketInput = new AddItemToBasketInput(); // AddItemToBasketInput | 

try {
    var result = api_instance.addItemToBasket(addItemToBasketInput);
    print(result);
} catch (e) {
    print("Exception when calling BasketApi->addItemToBasket: $e\n");
}

```

## Documentation for API Endpoints

All URIs are relative to *http://enigmatic-garden-23553.herokuapp.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BasketApi* | [**addItemToBasket**](doc//BasketApi.md#additemtobasket) | **post** /api/basket/addItem | 
*BasketApi* | [**basket**](doc//BasketApi.md#basket) | **get** /api/basket | 
*BasketApi* | [**checkout**](doc//BasketApi.md#checkout) | **post** /api/basket/checkout | 
*BasketApi* | [**removeItemFromBasket**](doc//BasketApi.md#removeitemfrombasket) | **post** /api/basket/removeItem | 
*CouriersApi* | [**acceptDeliveryRequest**](doc//CouriersApi.md#acceptdeliveryrequest) | **post** /api/couriers/{courierId}/requests/{orderId}/accept | 
*CouriersApi* | [**confirmDropoff**](doc//CouriersApi.md#confirmdropoff) | **post** /api/couriers/{courierId}/orders/{orderId}/confirmDropoff | 
*CouriersApi* | [**confirmOrderPickup**](doc//CouriersApi.md#confirmorderpickup) | **post** /api/couriers/{courierId}/orders/{orderId}/confirmPickup | 
*CouriersApi* | [**couriers**](doc//CouriersApi.md#couriers) | **get** /api/couriers | 
*CouriersApi* | [**createCourier**](doc//CouriersApi.md#createcourier) | **post** /api/couriers | 
*CouriersApi* | [**orders1**](doc//CouriersApi.md#orders1) | **get** /api/couriers/{courierId}/orders | 
*CouriersApi* | [**ownCourier**](doc//CouriersApi.md#owncourier) | **get** /api/couriers/me | 
*CouriersApi* | [**pendingDeliveryRequests**](doc//CouriersApi.md#pendingdeliveryrequests) | **get** /api/couriers/{courierId}/requests | 
*CouriersApi* | [**rejectDeliveryRequest**](doc//CouriersApi.md#rejectdeliveryrequest) | **post** /api/couriers/{courierId}/requests/{orderId}/reject | 
*CouriersApi* | [**startShift**](doc//CouriersApi.md#startshift) | **post** /api/couriers/{courierId}/startShift | 
*CouriersApi* | [**statistics**](doc//CouriersApi.md#statistics) | **get** /api/couriers/statistics | 
*CouriersApi* | [**stopShift**](doc//CouriersApi.md#stopshift) | **post** /api/couriers/{courierId}/stopShift | 
*CouriersApi* | [**updateLocation**](doc//CouriersApi.md#updatelocation) | **post** /api/couriers/{courierId}/location | 
*OrdersApi* | [**order**](doc//OrdersApi.md#order) | **get** /api/orders/{orderId} | 
*OrdersApi* | [**orders2**](doc//OrdersApi.md#orders2) | **get** /api/orders | 
*ProfileApi* | [**setAddress**](doc//ProfileApi.md#setaddress) | **post** /api/profile/address | 
*ProfileApi* | [**setPaymentMethod**](doc//ProfileApi.md#setpaymentmethod) | **post** /api/profile/payment_method | 
*RestaurantsApi* | [**createDish**](doc//RestaurantsApi.md#createdish) | **post** /api/restaurants/{restaurantId}/dishes | Create dish served by restaurant
*RestaurantsApi* | [**createRestaurant**](doc//RestaurantsApi.md#createrestaurant) | **post** /api/restaurants | Create new restaurant
*RestaurantsApi* | [**finishPreparingOrder**](doc//RestaurantsApi.md#finishpreparingorder) | **post** /api/restaurants/{restaurantId}/orders/{orderId}/finishPreparing | 
*RestaurantsApi* | [**orders**](doc//RestaurantsApi.md#orders) | **get** /api/restaurants/{restaurantId}/orders | 
*RestaurantsApi* | [**ownRestaurant**](doc//RestaurantsApi.md#ownrestaurant) | **get** /api/restaurants/me | 
*RestaurantsApi* | [**restaurant**](doc//RestaurantsApi.md#restaurant) | **get** /api/restaurants/{restaurantId} | Get restaurant info
*RestaurantsApi* | [**restaurantDishes**](doc//RestaurantsApi.md#restaurantdishes) | **get** /api/restaurants/{restaurantId}/dishes | Get restaurant dishes
*RestaurantsApi* | [**restaurants**](doc//RestaurantsApi.md#restaurants) | **get** /api/restaurants | Get list of restaurants
*RestaurantsApi* | [**startPreparingOrder**](doc//RestaurantsApi.md#startpreparingorder) | **post** /api/restaurants/{restaurantId}/orders/{orderId}/startPreparing | 


## Documentation For Models

 - [AddItemToBasketInput](doc//AddItemToBasketInput.md)
 - [Address](doc//Address.md)
 - [BasketDTO](doc//BasketDTO.md)
 - [BasketItemDTO](doc//BasketItemDTO.md)
 - [Courier](doc//Courier.md)
 - [CourierAdded](doc//CourierAdded.md)
 - [CourierLocationUpdated](doc//CourierLocationUpdated.md)
 - [CourierShiftStarted](doc//CourierShiftStarted.md)
 - [CourierShiftStopped](doc//CourierShiftStopped.md)
 - [CourierStatistics](doc//CourierStatistics.md)
 - [CreateCourierInput](doc//CreateCourierInput.md)
 - [CreateDishInput](doc//CreateDishInput.md)
 - [CreateRestaurantInput](doc//CreateRestaurantInput.md)
 - [DeliveryRequestDTO](doc//DeliveryRequestDTO.md)
 - [DeliveryRequested](doc//DeliveryRequested.md)
 - [DishDTO](doc//DishDTO.md)
 - [LatLng](doc//LatLng.md)
 - [MoneyView](doc//MoneyView.md)
 - [Order](doc//Order.md)
 - [OrderAssigned](doc//OrderAssigned.md)
 - [OrderCanceled](doc//OrderCanceled.md)
 - [OrderDelivered](doc//OrderDelivered.md)
 - [OrderItemDTO](doc//OrderItemDTO.md)
 - [OrderPickedUp](doc//OrderPickedUp.md)
 - [OrderPlaced](doc//OrderPlaced.md)
 - [OrderPreparationFinished](doc//OrderPreparationFinished.md)
 - [OrderPreparationStarted](doc//OrderPreparationStarted.md)
 - [OrderStatus](doc//OrderStatus.md)
 - [Profile](doc//Profile.md)
 - [RemoveFromBasketInput](doc//RemoveFromBasketInput.md)
 - [Restaurant](doc//Restaurant.md)
 - [RestaurantAdded](doc//RestaurantAdded.md)
 - [SetPaymentMethodInput](doc//SetPaymentMethodInput.md)
 - [UpdateLocationInput](doc//UpdateLocationInput.md)


## Documentation For Authorization


## JWT

- **Type**: HTTP basic authentication


## Author



