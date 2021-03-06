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


### Default Value
다트에서 취급하는 모든 타입은 객체이므로, 값을 할당하지 않은 변수는 모두 `null` 로 처리된다.

```dart
double pi;
assert(pi == null);
print(pi == null); // true
```

참고로 `assert` 메소드는 develop 에서만 동작하며 production code 에서는 메소드 동작을 무시한다.


### final and const
`final` 과 `const` 모두 다트에서 상수를 선언할때 사용된다. 차이점이라면 런타임에서 상수를 선언하느냐 컴파일 타임에서 상수를 선언하느냐의 차이가 있을것이다.

먼저 `final` 은 런타임에서 상수를 선언하기 위한 키워드다. 스위프트나 코틀린의 `let` 으로 생각해도 좋을것 같다.

`const` 는 컴파일 타임에 상수를 선언하고자 할때 사용된다. 컴파일 시점에 이미 상수임을 선언하는 것이기 때문에 런타임에서 결정이 되는 값들은 `const` 키워드를 사용할 수 없을 것이다. 따라서 주로 리터럴(숫자, 문자열) 상수를 선언하는데 사용될 것으로 보인다.
