# Dart

### Hello World
```dart
void main() {
  // Hello World
  print('Hello, World!');
}
```

### Variables
```dart
void main() {
  // Variables
  var message1 = 'Hello, World!';

  print(message1);

  var message2 = 'Hello, New World!';

  print(message2);

  message1 = 'Hello!';

  print(message1);
}
```

### Built-in types(int)
```dart
void main() {
  // int
  int number1 = 10;

  print(number1);

  int number2 = 20;

  print(number2);

  int number3 = -10;

  print(number3);
}
```

### Operators(additive, multiplicative)
```dart
void main() {
  // Operators(additive, multiplicative)
  int number1 = 10;
  int number2 = 20;

  print(number1 + number2);
  print(number1 - number2);
  print(number1 * number2);
  print(number1 / number2);
}
```

### Built-in types(double)
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

### Built-in types(bool)
```dart
void main() {
  // bool
  bool isTrue = true;
  bool isFalse = false;

  print(isTrue);
  print(isFalse);
}
```

### Built-in types(String)
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

### Built-in types(String)
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

### Built-in types(dynamic)
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

### Non-nullable and nullable types
```dart
void main() {
  // Non-nullable and nullable types
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

### Final and const
```dart
void main() {
  // Final and const
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
- `final`은 런타임에 값이 정해져도 괜찮습니다.
- `const`는 컴파일 타임에 값이 이미 결정되어 있어야 합니다.
- 따라서, `Datetime.now()`는 런타임에 호출되기 때문에, `const` 변수에 할당할 수 없고, `final` 변수에는 할당할 수 있습니다.

### Final and const
```dart
void main() {
  // Final and const
  final message1 = 'Hello, World!';

  print(message1);

  const message2 = 'Hello, New World!';

  print(message2);
}
```

### Operators(additive, multiplicative)
```dart
void main() {
  // Operators(additive, multiplicative)
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

### Operators(unary postfix, assignment)
```dart
void main() {
  // Operators(unary postfix, assignment)
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

### Operators(`??=` operator)
```dart
void main() {
  // Operators(`??=` operator)
  double? number = 10.0;

  print(number);

  number = 5.0;

  print(number);

  number = null;

  print(number);

  number ??= 100.0;

  print(number);
}
```
- 이 코드에서 `??=` 연산자는 널 병합 할당 연산자입니다. `number`가 `null`인 경우에만 `100.0`을 할당합니다. 만약 `number`가 이미 `null`이 아니라면 아무 일도 일어나지 않습니다.

### Operators(relational, equality)
```dart
void main() {
  // Operators(relational)
  int number1 = 1;
  int number2 = 2;

  print(number1 > number2);
  print(number1 < number2);
  print(number1 >= number2);
  print(number1 <= number2);
  print(number1 == number2);
  print(number1 != number2);
}
```

### Operators(type test)
```dart
void main() {
  // Operators(type test)
  int number = 1;

  print(number is int);
  print(number is String);

  print(number is! int);
  print(number is! String);
}
```

### Operators(logical AND, logical OR)
```dart
void main() {
  // Operators(logical AND, logical OR)
  bool result1 = 10 > 5 && 20 > 10 && 30 > 15;

  print(result1);

  bool result2 = 10 > 5 && 20 < 10;

  print(result2);

  bool result3 = 10 > 5 || 20 > 10;

  print(result3);

  bool result4 = 10 > 5 || 20 < 10;

  print(result4);

  bool result5 = 10 < 5 || 20 < 10;

  print(result5);
}
```

### Lists
```dart
void main() {
  // Lists
  List<String> alphabet = ['a', 'b', 'c', 'd', 'e'];
  List<int> number = [1, 2, 3, 4, 5];

  print(alphabet);
  print(number);

  // index
  print(alphabet[0]);
  print(alphabet[1]);
  print(alphabet[2]);
  print(alphabet[3]);
  print(alphabet[4]);
}
```

### Lists
```dart
void main() {
  // Lists
  List<String> alphabet = ['a', 'b', 'c', 'd', 'e'];
  
  print(alphabet.length);
  
  alphabet.add('f');
  
  print(alphabet);
  
  alphabet.remove('f');
  
  print(alphabet);
  
  print(alphabet.indexOf('c'));
}
```

### Maps
```dart
void main() {
  // Maps
  Map<String, String> dictionary = {
    'apple': '사과',
    'banana': '바나나',
    'orange': '오렌지',
  };

  print(dictionary);

  Map<String, bool> isFruit = {
    'apple': true,
    'banana': true,
    'orange': true,
    'computer': false,
  };

  print(isFruit);

  isFruit.addAll({
    'table': true,
  });

  print(isFruit);

  print(isFruit['computer']);

  isFruit['mango'] = true;

  print(isFruit);

  isFruit['table'] = false;

  print(isFruit);

  isFruit.remove('table');

  print(isFruit);

  print(isFruit.keys);
  print(isFruit.values);
}
```

### Sets
```dart
void main() {
  // Sets
  final Set<String> fruit = {
    'apple',
    'banana',
    'orange',
  };

  print(fruit);

  fruit.add('mango');

  print(fruit);

  fruit.remove('mango');

  print(fruit);

  print(fruit.contains('orange'));
}
```

### Control flow statements(if)
```dart
void main() {
  // Control flow statements(if)
  int number = 3;

  if (number % 2 == 0) {
    print('짝수입니다.');
  } else {
    print('홀수입니다.');
  }

  if (number % 3 == 0) {
    print('3으로 나눈 나머지가 0입니다.');
  } else if (number % 3 == 1) {
    print('3으로 나눈 나머지가 1입니다.');
  } else {
    print('3으로 나눈 나머지가 2입니다.');
  }
}
```

### Control flow statements(switch)
```dart
void main() {
  // Control flow statements(switch)
  int number = 2;

  switch (number % 3) {
    case 0:
      print('3으로 나눈 나머지가 0입니다.');
      break;

    case 1:
      print('3으로 나눈 나머지가 1입니다.');
      break;

    default:
      print('3으로 나눈 나머지가 2입니다.');
      break;
  }
}
```

### Control flow statements(For loops)
```dart
void main() {
  // Control flow statements(For loops)
  for (int i = 0; i < 10; i++) {
    print(i);
  }

  int sum = 0;
  List<int> numbers = [1, 2, 3, 4, 5];

  for (int i = 0; i < numbers.length; i++) {
    sum += numbers[i];
  }

  print(sum);

  sum = 0;

  // for in loop
  for (int number in numbers) {
    sum += number;
  }

  print(sum);
}
```

### Control flow statements(While and do-while)
```dart
void main() {
  // Control flow statements(While)
  int i = 0;

  while (i < 10) {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  }

  i = 0;

  // Control flow statements(Do-while)
  do {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  } while (i < 10);
}
```

### Control flow statements(Break and continue)
```dart
void main() {
  // Control flow statements(Break)
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      break;
    }

    print(i);
  }

  // Control flow statements(Continue)
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      continue;
    }

    print(i);
  }
}
```

### Enumerated types
```dart
// Enumerated types
enum Status {
  approved,
  pending,
  rejected,
}

void main() {
  Status status = Status.approved;

  if (status == Status.approved) {
    print('승인 상태입니다.');
  } else if (status == Status.pending) {
    print('대기 상태입니다.');
  } else {
    print('거절 상태입니다.');
  }
}
```

### Functions(Positional parameters)
```dart
void main() {
  // Functions(Positional parameters)
  add(10, 20, 30);

  add(1, 3, 5);
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positional parameter: 순서가 있는 파라미터
add(int x, int y, int z) {
  int sum = x + y + z;

  print('x: $x');
  print('y: $y');
  print('z: $z');

  if (sum % 2 == 0) {
    print('덧셈 결과가 짝수입니다.');
  } else {
    print('덧셈 결과가 홀수입니다.');
  }
}
```

### Functions(Optional parameters)
```dart
void main() {
  // Functions(Optional parameters)
  add(10);

  add(1, 3, 5);
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positional parameter: 순서가 있는 파라미터
// optional parameter: 있어도 되고 없어도 되는 선택적인 파라미터
add(int x, [int y = 20, int z = 30]) {
  int sum = x + y + z;

  print('x: $x');
  print('y: $y');
  print('z: $z');

  if (sum % 2 == 0) {
    print('덧셈 결과가 짝수입니다.');
  } else {
    print('덧셈 결과가 홀수입니다.');
  }
}
```

### Functions(Named parameters)
```dart
void main() {
  // Functions(Named parameters)
  add(x: 10, y: 20);

  add(x: 1, y: 3, z: 5);
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positional parameter: 순서가 있는 파라미터
// optional parameter: 있어도 되고 없어도 되는 선택적인 파라미터
// named parameter: 이름이 있는 파라미터(순서가 중요하지 않음)
add({
  required int x,
  required int y,
  int z = 30,
}) {
  int sum = x + y + z;

  print('x: $x');
  print('y: $y');
  print('z: $z');

  if (sum % 2 == 0) {
    print('덧셈 결과가 짝수입니다.');
  } else {
    print('덧셈 결과가 홀수입니다.');
  }
}
```

### Functions(Named parameters)
```dart
void main() {
  // Functions(Named parameters)
  add(x: 10, y: 20);

  add(x: 1, y: 3, z: 5);
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positional parameter: 순서가 있는 파라미터
// optional parameter: 있어도 되고 없어도 되는 선택적인 파라미터
// named parameter: 이름이 있는 파라미터(순서가 중요하지 않음)
add({
  required int x,
  required int y,
  int z = 30,
}) {
  int sum = x + y + z;

  print('x: $x');
  print('y: $y');
  print('z: $z');

  if (sum % 2 == 0) {
    print('덧셈 결과가 짝수입니다.');
  } else {
    print('덧셈 결과가 홀수입니다.');
  }
}
```

### Functions
```dart
void main() {
  // Functions
  int result1 = add(10, y: 20);
  int result2 = add(1, y: 3, z: 5);

  print('result1: $result1');
  print('result2: $result2');
  print('result1 + result2: ${result1 + result2}');
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positional parameter: 순서가 있는 파라미터
// optional parameter: 있어도 되고 없어도 되는 선택적인 파라미터
// named parameter: 이름이 있는 파라미터(순서가 중요하지 않음)
// arrow function(화살표 함수)
int add(
  int x, {
  required int y,
  int z = 30,
}) =>
    x + y + z;
```
- 화살표 함수는 함수 본문이 단일 표현식일 때 사용됩니다. `=>`는 `return`문과 동일하게 작동합니다.
- `() => x + y + z`는 `() { return x + y + z; }`와 동일합니다.
- 화살표 함수에서는 반환 값이 표현식으로 바로 반환되므로 `return` 키워드를 생략할 수 있습니다.

### Functions(Function types)
```dart
void main() {
  Operation operation = add;

  int result1 = operation(10, 20, 30);

  print(result1);

  operation = subtract;

  int result2 = operation(10, 20, 30);

  print(result2);

  int result3 = calculate(10, 20, 30, add);

  print(result3);

  int result4 = calculate(10, 20, 30, subtract);

  print(result4);
}

// signature
typedef Operation = int Function(int x, int y, int z);

int add(int x, int y, int z) => x + y + z;

int subtract(int x, int y, int z) => x - y - z;

int calculate(int x, int y, int z, Operation operation) => operation(x, y, z);
```

### 다양한 생성자를 활용한 클래스 설계 및 메서드 호출
```dart
void main() {
  Course course1 = Course('국어', 100000);

  print(course1.name);
  print(course1.price);
  course1.introduceName();
  course1.introducePrice();

  Course course2 = Course.customConstructor1('수학', 200000);

  print(course2.name);
  print(course2.price);
  course2.introduceName();
  course2.introducePrice();

  Course course3 = Course.customConstructor2(['영어', 300000]);

  print(course3.name);
  print(course3.price);
  course3.introduceName();
  course3.introducePrice();
}

class Course {
  String name;
  int price;

  Course(String name, int price)
      : this.name = name,
        this.price = price;

  Course.customConstructor1(this.name, this.price);

  Course.customConstructor2(List value)
      : this.name = value[0],
        this.price = value[1];

  void introduceName() {
    print('${this.name} 수업에 오신 것을 환영합니다.');
  }

  void introducePrice() {
    print('수강료는 ${this.price}원입니다.');
  }
}
```

```dart
void main() {
  Course course1 = Course('국어', 100000);

  print(course1.name);
  print(course1.price);
  course1.introduceName();
  course1.introducePrice();

  Course course2 = Course.customConstructor1('수학', 200000);

  print(course2.name);
  print(course2.price);
  course2.introduceName();
  course2.introducePrice();

  Course course3 = Course.customConstructor2(['영어', 300000]);

  print(course3.name);
  print(course3.price);
  course3.introduceName();
  course3.introducePrice();
}

class Course {
  final String name;
  final int price;

  const Course(String name, int price)
      : this.name = name,
        this.price = price;

  Course.customConstructor1(this.name, this.price);

  Course.customConstructor2(List value)
      : this.name = value[0],
        this.price = value[1];

  void introduceName() {
    print('${this.name} 수업에 오신 것을 환영합니다.');
  }

  void introducePrice() {
    print('수강료는 ${this.price}원입니다.');
  }
}
```
