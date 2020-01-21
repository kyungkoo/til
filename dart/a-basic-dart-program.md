# A toure of the Dart language
## [A basic Dart program](https://dart.dev/guides/language/language-tour#a-basic-dart-program)

```dart
// Define a function.
printInteger(int aNumber) {
  print('The number is $aNumber.'); // Print to console.
}

// This is where the app starts executing.
main() {
  var number = 42; // Declare and initialize a variable.
  printInteger(number); // Call a function.
}
```

- 다트는 프로그램의 시작점이 되는 `main` 함수를 갖는다.
- 다트에서 함수 정의 시, 반환 타입을 생략해도 되는 것으로 보인다.([Functions](https://dart.dev/guides/language/language-tour#functions) 절에서 좀 더 살펴봐야 할듯)
- `print` 함수를 통해 콘솔로 출력이 가능하다.
- `$변수명` 또는 `${표현식}` 을 통해 문자열에 수식이나 변수를 바로 삽입할 수 있다.
- 변수를 선언할 때 타입을 앞에 써준다 ex>`int aNumber`.
- 타입을 생략할 때에는 `var` 를 써준다.ex> `var number`.
- 타입을 생략하면 초기화 값을 통해 타입 추론이 가능하다.