# APIs

#### Adding APIs to Gitbook

{% api-method method="get" host="https:weather.api.here.com" path="/weather/1.0/report.json" %}
{% api-method-summary %}
Collect weather Information
{% endapi-method-summary %}

{% api-method-description %}
Query to collect weather information about a particular location
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="app\_id" type="string" required=true %}
Your APP ID
{% endapi-method-parameter %}

{% api-method-parameter name="app\_code" type="string" required=true %}
Your APP CODE
{% endapi-method-parameter %}

{% api-method-parameter name="product" type="string" required=true %}
nws\_alert
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}
Location name: eg. Lufkin, Tx
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

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
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

