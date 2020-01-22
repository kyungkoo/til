## [Variables](https://dart.dev/guides/language/language-tour#variables)

```dart
var lastName = "Kang";
String firstName = 'Kyungkoo';
dynamic country = 'Korea';
```

다트는 크게 세 가지 방식으로 변수를 선언할 수 있다.
첫 번째는 `var` 키워드를 사용하는 방법으로, 변수의 타입은 대입하는 값에 의해 정해진다.
두 번째로 타입을 직접 선언하는 방법이 있다.
`String` 타입을 명시함으로써 해당 변수의 타입을 설정할 수 있다.
세 번째는 `dynamic` 키워드를 사용하는 방법이다. 이 역시 `var` 와 마찬가지로 대입하는 값에 따라 변수 타입이 결정된다.

마지막으로 위 방법 이외에 `Object` 키워드를 사용하여 `Object language = "dart";` 와 같이 선언하는 방법도 있다.

[가이드 라인](https://dart.dev/guides/language/effective-dart/design#do-annotate-with-object-instead-of-dynamic-to-indicate-any-object-is-allowed)에 따르면 `dynamic` 보다는 `Object` 를 추천하는 것으로 보이는데 정확한 이유는 좀 더 확인해 보아야 할듯 하다. 
