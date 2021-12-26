<p align="center">
  <img src="https://github.com/ayhanunal/BasketLayout/blob/master/art/basketlayout-wip.gif" width=300 height=600>
</p>

## maximum quantity filter for basket

```kotlin
maxBasketLimit?.let {
  if ((quantity + incrementValue) > it){
    listener?.maxLimitExceeded()
  }else{
    listener?.onClickIncreaseQuantity(quantity + incrementValue)
    setLoading()
  }
}
if (maxBasketLimit == null) {
  listener?.onClickIncreaseQuantity(quantity + incrementValue)
  setLoading()
}
```
<p align="center">
  <img src="https://github.com/ayhanunal/BasketLayout/blob/master/art/max_limit_alert.png" width=300 height=600>
</p>
