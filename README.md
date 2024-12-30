# dart

```dart
void main() {
  print('Hello, World!');
}
```

```dart
void main() {
  // variable
  var message1 = 'Hello, World!';

  print(message1);

  var message2 = 'Hello, New World!';

  print(message2);

  message1 = 'Hello!';

  print(message1);
}

```

```dart
void main() {
  // integer
  int number1 = 10;

  print(number1);

  int number2 = 20;

  print(number2);

  int number3 = -10;

  print(number3);
}
```

```dart
void main() {
  // integer
  int number1 = 10;
  int number2 = 20;

  print(number1 + number2);
  print(number1 - number2);
  print(number1 * number2);
  print(number1 / number2);
}
```

```dart
void main() {
  // double
  double number1 = 7.5;
  double number2 = 2.5;

  print(number1 + number2);
  print(number1 - number2);
  print(number1 * number2);
  print(number1 / number2);
}
```

```dart
void main() {
  // boolean
  bool isTrue = true;
  bool isFalse = false;

  print(isTrue);
  print(isFalse);
}
```

```dart
void main() {
  // String
  String message1 = 'Hello, World!';
  String message2 = 'Hello, New World!';

  print(message1);
  print(message2);

  var message3 = 'Hello!';
  var number = 10;

  print(message3.runtimeType);
  print(number.runtimeType);

  // Map<String, Map<int, List<double>>> test = {};
  var test = {};

  print(test.runtimeType);
}
```

```dart
void main() {
  // String
  String message1 = 'Hello,';
  String message2 = 'World!';

  print(message1 + message2);
  print(message1 + ' ' + message2);

  print('${message1} ${message2}');
  print('$message1 $message2');

  print('${message1.runtimeType}');
  print('$message1.runtimeType');
}
```

```dart
void main() {
  // dynamic
  dynamic message1 = 'Hello, World!';

  print(message1);

  dynamic number = 10;

  print(number);

  var message2 = 'Hello, New World!';

  print(message2);

  print(message1.runtimeType);
  print(message2.runtimeType);

  message1 = 10;
  // message2 = 10;
}
```

```dart
void main() {
  // nullable, non-nullable
  String message1 = 'Hello, World!';

  // message1 = null;

  print(message1);

  String? message2 = 'Hello, New World!';

  message2 = null;

  print(message2);

  message2 = 'Hello!';

  print(message1!);
  print(message2!);
}
```

```dart
void main() {
  // final, const
  final String message1 = 'Hello, World!';

  print(message1);

  const String message2 = 'Hello, New World!';

  print(message2);

  // message1 = 'Hello!';
  // message2 = 'Hello!';

  final DateTime time1 = DateTime.now();
  // const DateTime time2 = DateTime.now();

  print(time1);
}
```

```dart
void main() {
  // final, const
  final message1 = 'Hello, World!';

  print(message1);

  const message2 = 'Hello, New World!';

  print(message2);
}
```

```dart
void main() {
  // operator
  int number = 10;
  
  print(number + 2);
  print(number - 2);
  print(number * 2);
  print(number / 2);
  print(number);
  
  print(number % 2);
  print(number % 3);
  print(number);
}
```

```dart
void main() {
  // operator
  double number = 10.0;

  number++;

  print(number);

  number--;

  print(number);

  number += 5;

  print(number);

  number -= 5;

  print(number);

  number *= 5;

  print(number);

  number /= 5;

  print(number);
}
```
