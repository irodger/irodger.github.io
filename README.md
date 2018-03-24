# irodger.github.io
## XLSX-JSON parser
Simple xlsx to json parser. Also support i18next format. Relies on node-xlsx.
* [GitHub](https://github.com/irodger/xlsx-json-parser)
* [NPM](https://www.npmjs.com/package/xlsx-json-parser)
```js
{
  "lang": {
    "translations": {
      "key": "value",
      "another_key": "another value"
    }
  }
}
```

## Price Like Human's
#### JavaScript Kit for formatting price or numbers to human likes format. Actually for cryptocurrency with 7+ numbers after delimiter
* [GitHub](https://github.com/irodger/price-like-humans)
* [NPM](https://www.npmjs.com/package/price-like-humans)
### Example
```js
priceLikeHumans.formattedPrice(12345.6789) 
//> EU Locale "12,345.678,9"
//> RU Locale "12 345.678 9"
```
```js
priceLikeHumans.exponentFormatter(1e-7) 
//> "0.0000001"
```
```js
priceLikeHumans.excessZeroes(10e-8) 
//> 1e-7
```
```js
priceLikeHumans.exponentFormatter( priceLikeHumans.excessZeroes(10e-8) )
//> "0.0000001"
```
```js
priceLikeHumans.formattedPrice( 
  priceLikeHumans.exponentFormatter( 
    priceLikeHumans.excessZeroes(10e-8) 
  ) 
)
//> "0.000 000 1"
```
