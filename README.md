---
description: Investigation on Gitbook Features
---

# Gitbook Spike

1. **Images**

![](.gitbook/assets/pexels-photo-120049.jpeg)

#### 2. Iframes

To add a rich embed, simply paste the link of the content you want to embed, then press `ENTER` and voilà. For ex. below content is loaded from url: [https://www.here.com](https://www.here.com)

{% embed url="https://www.here.com" %}

####  

#### 3. Code Block

{% code-tabs %}
{% code-tabs-item title="index.html" %}
```markup
<!DOCTYPE html>
  <html>
  <head>
  ...
  <meta name="viewport" content="initial-scale=1.0, width=device-width"/>
  <script src="https://js.api.here.com/v3/3.1/mapsjs-core.js"
     type="text/javascript" charset="utf-8"></script>
  <script src="https://js.api.here.com/v3/3.1/mapsjs-service.js"
     type="text/javascript" charset="utf-8"></script>
  <script src="https://js.api.here.com/v3/3.1/mapsjs-mapevents.js"
     type="text/javascript" charset="utf-8"></script>
  ...
  </head>
```
{% endcode-tabs-item %}
{% endcode-tabs %}



#### 4.  Code Block with Tabs

{% code-tabs %}
{% code-tabs-item title="Scala" %}
```scala
// If you comment out this line, the application will continue to publish a new version
// to the output catalog once per minute, until you explicitly kill the application if
// running locally, or cancel the pipeline version if running on Pipeline Service.
throw new InterruptedException("Halting stream processing")

```
{% endcode-tabs-item %}

{% code-tabs-item title=undefined %}
```java
// If you comment out this line, the application will continue to publish a new
// version to the output catalog once per minute, until you explicitly kill
// the application if running locally, or cancel the pipeline version if
// running on Pipeline Service.
throw new InterruptedException("Halting stream processing");

```
{% endcode-tabs-item %}
{% endcode-tabs %}



#### 5. Code editing with CodePen

{% embed url="https://codepen.io/davidkpiano/pen/wMqXea" %}



#### 6. Videos \( youtube\)

To add a rich embed, simply paste the link of the content you want to embed, then press `ENTER` and voilà. For ex. below video is loaded from url:  [https://www.youtube.com/watch?v=54J\_ZCbeJdc](https://www.youtube.com/watch?v=54J_ZCbeJdc)

{% embed url="https://www.youtube.com/watch?v=54J\_ZCbeJdc" %}



#### 7. APIs

{% api-method method="get" host="https://weather.api.here.com" path="/weather/1.0/report.json" %}
{% api-method-summary %}
Collect weather Informations
{% endapi-method-summary %}

{% api-method-description %}
Query provides weather warning and information about a particular location.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="app\_code" type="string" required=true %}
Your APP CODE
{% endapi-method-parameter %}

{% api-method-parameter name="app\_id" type="string" required=true %}
Your APP ID
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}
Location name: eg. Lufkin, Tx
{% endapi-method-parameter %}

{% api-method-parameter name="product" type="string" required=true %}
nws\_alerts
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

{% code-tabs %}
{% code-tabs-item title="Response.json" %}
```
{
  "nwsAlerts": {
  "warning": [
    {
    "type": "6",
    "description": "FLOOD STATEMENT",
    "severity": 11,
    "message": "959 AM CDT MON MAY 19 2014 THE FLOOD WARNING CONTINUES FOR THE ANGELINA RIVER NEAR LUFKIN TEXAS. UNTIL FURTHER NOTICE...OR UNTIL THE WARNING IS CANCELLED. AT 715 AM MONDAY THE STAGE WAS 11.5 FEET. MINOR FLOODING IS OCCURRING AND MINOR FLOODING IS FORECAST. FLOOD STAGE IS 10 FEET. FORECAST...EXPECT LITTLE CHANGE THROUGH TUESDAY MORNING. IMPACT...MINOR LOWLAND FLOODING.",
    "county": [
      {
      "value": "TXC005",
      "country": "US",
      "countryName": "United States",
      "state": "TX",
      "stateName": "Texas",
      "name": "Angelina",
      "latitude": 31.28145,
      "longitude": -94.56949
      }]
    }]
  }}
```
{% endcode-tabs-item %}
{% endcode-tabs %}
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



#### 8. Hints

{% hint style="success" %}
Sample Hint 1
{% endhint %}

{% hint style="danger" %}
Sample Hint 2
{% endhint %}

{% hint style="info" %}
Sample Hint 3
{% endhint %}



#### 9. Files

{% file src=".gitbook/assets/sample.txt" %}





