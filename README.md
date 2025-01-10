# Dart

### Introduction to Dart(Hello World)
```dart
void main() {
  // Introduction to Dart(Hello World)
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
  // Built-in types(int)
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
  // Built-in types(double)
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
  // Built-in types(bool)
  bool isTrue = true;
  bool isFalse = false;

  print(isTrue);
  print(isFalse);
}
```

### Built-in types(String)
```dart
void main() {
  // Built-in types(String)
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
- `var`는 타입이 아니며, 타입을 추론하는 키워드입니다.
- 가독성과 유지보수를 위해 타입을 명시적으로 작성하는 것이 좋습니다.
- 긴 타입 이름을 간결하게 작성하려면 `var`를 사용하는 것이 좋습니다.

### Built-in types(String)
```dart
void main() {
  // Built-in types(String)
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
  // Built-in types(dynamic)
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
- `dynamic`: 처음 선언한 타입이 고정되지 않으며, 이후 다른 타입으로 변경 가능합니다. 타입 안전성을 포기하고 유연성을 얻습니다.
- `var`: 첫 할당 시점의 타입으로 고정되며, 이후 다른 타입으로 변경할 수 없습니다. 타입 안정성을 유지하며 코드가 간결해집니다.

### Understanding null safety(Non-nullable and nullable types)
```dart
void main() {
  // Understanding null safety(Non-nullable and nullable types)
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
- 모든 타입은 해당 타입만 할당될 수 있는 non-nullable 타입과, `null`도 함께 할당될 수 있는 nullable 타입으로 나뉩니다.
- `?` 키워드를 사용하면 null을 할당할 수 있는 nullable 타입으로 선언됩니다.
- `!` 키워드를 사용하면 null이 아님을 보장할 수 있으며, 실제로 null인 경우 런타임 에러가 발생합니다.

### Variables(Final and const)
```dart
void main() {
  // Variables(Final and const)
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

### Variables(Final and const)
```dart
void main() {
  // Variables(Final and const)
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
  // Operators(relational, equality)
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

### Collections(Lists)
```dart
void main() {
  // Collections(Lists)
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

### Collections(Lists)
```dart
void main() {
  // Collections(Lists)
  List<String> alphabet = ['a', 'b', 'c', 'd', 'e'];
  
  print(alphabet.length);
  
  alphabet.add('f');
  
  print(alphabet);
  
  alphabet.remove('f');
  
  print(alphabet);
  
  print(alphabet.indexOf('c'));
}
```

### Collections(Maps)
```dart
void main() {
  // Collections(Maps)
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

### Collections(Sets)
```dart
void main() {
  // Collections(Sets)
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

### Branches(If)
```dart
void main() {
  // Branches(If)
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

### Branches(Switch statements)
```dart
void main() {
  // Branches(Switch statements)
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

### Loops(For loops)
```dart
void main() {
  // Loops(For loops)
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

  for (int number in numbers) {
    sum += number;
  }

  print(sum);
}
```

### Loops(While and do-while)
```dart
void main() {
  // Loops(While and do-while)
  int i = 0;

  while (i < 10) {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  }

  i = 0;

  do {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  } while (i < 10);
}
```

### Loops(Break and continue)
```dart
void main() {
  // Loops(Break and continue)
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      break;
    }

    print(i);
  }

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
- `enum`은 데이터의 수와 종류를 제한하여 강제하기 위해 사용됩니다.

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
- 함수의 목적, 파라미터, 반환값, 테스트 케이스를 미리 작성한 후 구현하는 것이 좋습니다.

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
  int z = 30, // `required` 키워드가 없으면 optional parameter입니다.
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
  // Functions(Function types)
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

### Classes(Using constructors)
```dart
void main() {
  // Classes(Using constructors)
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

### Classes(Using constructors)
```dart
void main() {
  // Classes(Using constructors)
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
- Dart에서 `final`로 선언된 변수는 생성자에서 값을 초기화할 수 있지만, 한 번 설정된 값은 변경할 수 없습니다. 이는 불변성을 보장합니다.

### Classes(Using constructors)
```dart
void main() {
  // Classes(Using constructors)
  Course course1 = const Course('국어', 100000);

  print(course1.name);
  print(course1.price);
  course1.introduceName();
  course1.introducePrice();

  Course sameCourse1 = const Course('국어', 100000);

  print(course1 == sameCourse1); // true

  Course course2 = Course.customConstructor1('수학', 200000);

  print(course2);

  Course course3 = Course.customConstructor2(['영어', 300000]);

  print(course3);
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
- Dart에서 `const constructor`를 사용하면 클래스의 모든 필드가 `final`이어야 하며, 이는 해당 클래스가 컴파일 타임 상수로 처리될 수 있도록 보장합니다.
- Flutter에서 위젯을 작성할 때 `const`를 활용하면, 동일한 값의 인스턴스를 재사용하여 메모리와 성능을 최적화할 수 있습니다. 이는 특히 Flutter에서 빌드 트리가 반복적으로 재생성되는 상황에서 효과적입니다.
- 위젯 트리가 업데이트될 때 Flutter는 기존 트리와 새로 생성된 트리를 비교하여 어떤 위젯이 변경되었는지 판단합니다. 변경된 위젯만 새로 렌더링하고, 나머지는 재사용하거나 그대로 둡니다.
- `const` 키워드를 사용하면 컴파일 타임에 메모리에 고정되며, 이후 동일한 내용을 가진 위젯이 재생성될 필요가 없습니다. 빌드가 반복되더라도 기존 메모리를 재사용합니다. `const` 키워드를 사용하지 않으면 매 빌드 시 Flutter는 항상 새로운 객체를 생성합니다. 이로 인해 메모리 사용량이 증가하고, 비교 작업에도 시간이 더 소요됩니다. `const` 위젯은 내용이 같으면 참조도 같기 때문에 Flutter가 참조만 비교하면 되지만, `const`가 아닌 위젯은 내용이 같아도 참조가 다르기 때문에 Flutter가 내용도 비교해야 하기 때문입니다.
- `const` 키워드를 사용하지 않으면 Dart는 각 인스턴스를 별도의 객체로 생성하므로, 같은 내용이라도 서로 다른 메모리 주소를 가지게 됩니다. 반면, `const` 키워드를 사용하여 생성한 인스턴스는 컴파일 타임 상수로 간주되며, 같은 내용의 상수는 동일한 메모리 주소를 공유하게 됩니다.

### Methods(Getters and setters)
```dart
void main() {
  // Methods(Getters and setters)
  Course course1 = Course('국어', 100000);

  Course course2 = Course.customConstructor1('수학', 200000);

  Course course3 = Course.customConstructor2(['영어', 300000]);

  print(course1.getName);
  print(course2.getName);
  print(course3.getName);

  course1.setName = '언어';
  print(course1.getName);
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

  // getter
  String get getName {
    return this.name;
  }

  // setter
  set setName(String name) {
    this.name = name;
  }
}
```
- Getter는 간단한 값 반환에 적합하고, 함수는 더 복잡한 로직에 적합합니다.
- Setter를 사용하는 대신 `final`을 활용하여 상태 변화를 줄이는 것이 선호됩니다.

### Libraries & imports(public, private)
```dart
void main() {
  // Libraries & imports(public, private)
  _Course course1 = _Course('국어', 100000);

  _Course course2 = _Course.customConstructor1('수학', 200000);

  _Course course3 = _Course.customConstructor2(['영어', 300000]);

  print(course1.getName);
  print(course2.getName);
  print(course3.getName);

  course1.setName = '언어';
  print(course1.getName);
}

class _Course {
  String name;
  int price;

  _Course(String name, int price)
      : this.name = name,
        this.price = price;

  _Course.customConstructor1(this.name, this.price);

  _Course.customConstructor2(List value)
      : this.name = value[0],
        this.price = value[1];

  void introduceName() {
    print('${this.name} 수업에 오신 것을 환영합니다.');
  }

  void introducePrice() {
    print('수강료는 ${this.price}원입니다.');
  }

  // getter
  String get getName {
    return this.name;
  }

  // setter
  set setName(String name) {
    this.name = name;
  }
}
```
- Dart에서 하나의 파일은 하나의 라이브러리로 간주됩니다. 따라서 `_`는 파일 단위로 private를 설정하는 역할을 합니다. 다른 파일에서 해당 라이브러리를 `import`하더라도 `_`로 시작하는 요소는 접근할 수 없습니다.

### Classes(Inheritance)
```dart
void main() {
  // Classes(Inheritance)
  Course course = const Course(name: '수학', price: 300000);

  course.sayCoursePrice();

  HighCourse highCourse = const HighCourse('고등수학', 500000);

  highCourse.sayCoursePrice();
  highCourse.sayHighCourse();

  MiddleCourse middleCourse = const MiddleCourse('중등수학', 200000);

  middleCourse.sayCoursePrice();
  middleCourse.sayMiddleCourse();

  print('----- Type Comparison -----');
  print(course is Course);
  print(course is HighCourse);
  print(course is MiddleCourse);

  print(highCourse is Course);
  print(highCourse is HighCourse);
  print(highCourse is MiddleCourse);

  print(middleCourse is Course);
  print(middleCourse is HighCourse);
  print(middleCourse is MiddleCourse);
}

class Course {
  final String name;
  final int price;

  const Course({
    required this.name,
    required this.price,
  });

  void sayCourseName() {
    print('${this.name} 수업에 오신 것을 환영합니다.');
  }

  void sayCoursePrice() {
    print('${this.name} 수업의 수강료는 ${this.price}원입니다.');
  }
}

class HighCourse extends Course {
  const HighCourse(String name, int price) : super(name: name, price: price);

  void sayHighCourse() {
    print('고등 과정입니다.');
  }
}

class MiddleCourse extends Course {
  const MiddleCourse(String name, int price) : super(name: name, price: price);

  void sayMiddleCourse() {
    print('중등 과정입니다.');
  }
}
```
- 자식 클래스는 부모 클래스의 모든 public 및 protected 속성을 상속받습니다.
- 부모 클래스의 생성자가 초기화된 속성을 가진 경우, `super`를 통해 호출해야 합니다.

### Extend a class(Overriding members)
```dart
void main() {
  // Extend a class(Overriding members)
  TimesTwo timesTwo = TimesTwo(2);

  print(timesTwo.calculate());

  TimesTen timesFive = TimesTen(2);

  print(timesFive.calculate());
}

// method - function(class 내부에 있는 함수)
// override - 덮어쓰다(우선시하다)
class TimesTwo {
  final int number;

  TimesTwo(this.number);

  // method
  int calculate() {
    return number * 2;
  }
}

class TimesTen extends TimesTwo {
  TimesTen(int number) : super(number);

  @override
  int calculate() {
    return super.calculate() * 5;
  }
}
```
### Static variables and methods
```dart
void main() {
  // Static variables and methods
  Employee employee1 = Employee('name1');
  Employee employee2 = Employee('name2');

  employee1.printNameAndBuilding(); // instance에 귀속
  employee2.printNameAndBuilding(); // instance에 귀속

  Employee.building = 'building'; // class에 귀속

  employee1.printNameAndBuilding(); // instance에 귀속
  employee2.printNameAndBuilding(); // instance에 귀속

  Employee.printBuilding(); // class에 귀속
}

class Employee {
  // 직원이 일하는 건물
  static String? building;
  // 직원 이름
  final String name;

  Employee(
    this.name,
  );

  void printNameAndBuilding() {
    print('직원명: $name, 근무지: $building');
  }

  static void printBuilding() {
    print('근무지: $building');
  }
}
```
- `static` 키워드는 instance에 속하지 않고 class에 속하는 멤버를 정의합니다.

### Interfaces and abstract classes
```dart
void main() {
  // Interfaces and abstract classes
  BoyGroup bts = BoyGroup('bts');
  GirlGroup blackpink = GirlGroup('blackpink');

  bts.sayName();
  blackpink.sayName();

  print(bts is IdolInterface);
  print(bts is BoyGroup);
  print(bts is GirlGroup);

  print(blackpink is IdolInterface);
  print(blackpink is BoyGroup);
  print(blackpink is GirlGroup);
}

abstract class IdolInterface {
  String name;

  IdolInterface(this.name);

  void sayName();
}

class BoyGroup implements IdolInterface {
  String name;

  BoyGroup(this.name);

  void sayName() {
    print('안녕하세요. $name입니다.');
  }
}

class GirlGroup implements IdolInterface {
  String name;

  GirlGroup(this.name);

  void sayName() {
    print('안녕하세요. $name입니다.');
  }
}
```
- Dart에서 클래스나 추상 클래스를 `implements` 키워드를 통해 인터페이스처럼 사용할 수 있습니다.
- `abstract` 키워드는 클래스가 추상적임을 나타내며, 이 클래스로는 인스턴스를 생성할 수 없습니다. 또한, 추상 클래스는 구현되지 않은 메서드를 포함할 수 있으며, 이를 서브클래스에서 반드시 구현해야 합니다.

### Generics
```dart
void main() {
  Lecture<String, String> lecture1 = Lecture('123', 'lecture1');

  lecture1.printIdType();

  Lecture<int, String> lecture2 = Lecture(123, 'lecture2');

  lecture2.printIdType();
}

class Lecture<T, X> {
  final T id;
  final X name;

  Lecture(this.id, this.name);

  void printIdType() {
    print(id.runtimeType);
  }
}
```
- 제네릭(Generic)은 클래스나 함수에서 사용할 데이터의 타입을 외부에서 지정할 수 있도록 하는 기능입니다.

### Object oriented programming
```dart
void main() {
  Test test = Test();

  print(test.hashCode);
  print(test.runtimeType);
  print(test.toString());
}

// Object Oriented Programming(OOP)
// 객체지향 프로그래밍
class Test {}
```
- Dart에서는 모든 클래스가 기본적으로 `Object` 클래스를 상속받습니다.

### Converting between list, map, and set
```dart
void main() {
  // Converting between list, map, and set
  List<String> blackpink = ['로제', '지수', '리사', '제니', '제니'];

  print(blackpink);
  print(blackpink.asMap());
  print(blackpink.toSet());

  Map blackpinkMap = blackpink.asMap();

  print(blackpinkMap);
  print(blackpinkMap.keys.toList());
  print(blackpinkMap.values.toList());

  Set blackpinkSet = Set.from(blackpink);

  print(blackpinkSet);
  print(blackpinkSet.toList());
}
```

### Using dart's `map` method
```dart
void main() {
  // Using dart's `map` method
  List<String> blackpink = ['로제', '지수', '리사', '제니'];

  final newBlackpink = blackpink.map((x) {
    return '블랙핑크 $x';
  });

  print(blackpink);
  print(newBlackpink);

  final newBlackpink2 = blackpink.map((x) => '블랙핑크 $x');

  print(newBlackpink2.toList());

  print(blackpink == blackpink);
  print(blackpink == newBlackpink);
  print(newBlackpink == newBlackpink2);

  // [1.jpg, 3.jpg, 5.jpg, 7.jpg, 9.jpg]
  String number = '13579';

  final parsed = number.split('').map((x) => '$x.jpg').toList();

  print(parsed);
}
```
- Dart의 `map` 함수는 기존 리스트를 변경하지 않고, 새로운 Iterable 객체를 생성합니다.

### Using dart's `map` method
```dart
void main() {
  // Using dart's `map` method
  Map<String, String> harryPotter = {
    'Harry Potter': '해리 포터',
    'Ron Weasley': '론 위즐리',
    'Hermione Granger': '헤르미온느 그레인저',
  };

  final result = harryPotter.map((key, value) => MapEntry(
        'Harry Potter Character $key',
        '해리 포터 캐릭터 $value',
      ));

  print(harryPotter);
  print(result);

  final keys = harryPotter.keys.map((x) => 'HPC $x').toList();
  final values = harryPotter.values.map((x) => '해리 포터 캐릭터 $x').toList();

  print(keys);
  print(values);
}
```

### Using dart's `map` method
```dart
void main() {
  // Using dart's `map` method
  Set<String> blackpinkSet = {'로제', '지수', '제니', '리사'};

  final newSet = blackpinkSet.map((x) => '블랙핑크 $x').toList();

  print(newSet);
}
```

### Using dart's `where` method
```dart
void main() {
  // Using dart's `where` method
  List<Map<String, String>> people = [
    {
      'name': '로제',
      'group': '블랙핑크',
    },
    {
      'name': '지수',
      'group': '블랙핑크',
    },
    {
      'name': '진',
      'group': '방탄소년단',
    },
    {
      'name': '정국',
      'group': '방탄소년단',
    },
  ];

  print(people);

  final blackpink = people.where((x) => x['group'] == '블랙핑크');
  final bts = people.where((x) => x['group'] == '방탄소년단');

  print(blackpink);
  print(bts);
}
```

### Using dart's `reduce` method
```dart
void main() {
  // Using dart's `reduce` method
  List<int> numbers = [1, 3, 5, 7, 9];

  final sum = numbers.reduce((prev, next) {
    print('----------');
    print('prev: $prev');
    print('next: $next');
    print('prev + next: ${prev + next}');

    return prev + next;
  });

  print(sum);

  List<String> words = [
    '안녕하세요 ',
    '저는 ',
    '학생입니다.',
  ];

  final sentence = words.reduce((prev, next) =>
      prev +
      next);

  print(sentence);
}
```
- `reduce`는 리스트 아이템의 타입에 따라 반환 타입이 결정되며, 그 타입에 맞춰 결과가 반환됩니다.

### Using dart's `fold` method
```dart
void main() {
  // Using dart's `fold` method
  List<int> numbers = [1, 3, 5, 7, 9];

  final sum = numbers.fold<int>(0, (prev, next) {
    print('prev: $prev');
    print('next: $next');
    print('prev + next: ${prev + next}');

    return prev + next;
  });

  print(sum);

  List<String> words = [
    '안녕하세요 ',
    '저는 ',
    '학생입니다.',
  ];

  final sentence = words.fold<String>('', (prev, next) => prev + next);

  print(sentence);

  final count = words.fold<int>(
      0,
      (prev, next) =>
          prev +
          next.length);

  print(count);
}
```
- `fold` 함수는 `reduce`와 달리 반환 타입이 고정되지 않으며, 원하는 타입을 명시할 수 있습니다. `fold`는 초기 값과 결합 함수 두 가지를 받기 때문에, 초기 값의 타입을 기준으로 반환 타입을 지정할 수 있습니다.

### Using the spread operator
```dart
void main() {
  // Using the spread operator
  List<int> even = [2, 4, 6, 8];

  List<int> odd = [1, 3, 5, 7, 9];

  print([...even, ...odd]);
  print(even);
  print([...even]);
  print(even == [...even]);
}
```
- `Spread operator`로 복사한 리스트는 새로운 주소를 가지게 됩니다.

### Functional programming
```dart
void main() {
  // Functional programming
  final List<Map<String, String>> people = [
    {
      'name': '로제',
      'group': '블랙핑크',
    },
    {
      'name': '지수',
      'group': '블랙핑크',
    },
    {
      'name': '진',
      'group': '방탄소년단',
    },
    {
      'name': '정국',
      'group': '방탄소년단',
    },
  ];

  print(people);

  final parsedPeople = people
      .map((x) => Person(
            name: x['name']!,
            group: x['group']!,
          ))
      .toList();

  print(parsedPeople);

  final bts = parsedPeople.where((x) => x.group == '방탄소년단').toList();

  print(bts);

  final result = people
      .map((x) => Person(
            name: x['name']!,
            group: x['group']!,
          ))
      .where((x) => x.group == '방탄소년단')
      .toList()
      .fold<int>(0, (prev, next) => prev + next.name.length);

  print(result);
}

class Person {
  final String name;
  final String group;

  Person({
    required this.name,
    required this.group,
  });

  String toString() {
    return 'name: $name, group: $group';
  }
}
```
- Map 형태의 데이터는 동적으로 값을 저장하기 때문에, 특정 키가 존재하는지, 값이 올바른지, 키 이름에 오타가 없는지 등을 컴파일 타임에 확인하기 어려운 문제가 있습니다. 예를 들어, 서버에서 JSON 형태로 데이터를 받아올 때, 데이터 구조가 일관되지 않거나 예기치 못한 키가 있을 수 있습니다.
- 클래스를 사용한 형변환을 통해 정확한 타입 검증을 할 수 있습니다. 이를 통해 데이터가 예상된 구조와 일치하는지 확인할 수 있고, 오타나 잘못된 키를 사전에 처리할 수 있습니다.
- 클래스로 형변환하면, 데이터를 다루는 데 있어 타입 안정성을 높이고, 코드에서 실수를 줄이며, IDE의 자동완성 및 타입 검사를 활용할 수 있습니다.

### Synchronous programming
```dart
void main() {
  // Synchronous programming
  addNumbers(1, 1);
  addNumbers(2, 2);
}

// 1 + 1 = 2
// 2 + 2 = 4
void addNumbers(int number1, int number2) {
  print('계산 중: $number1 + $number2');

  print('계산 완료: ${number1 + number2}');
}
```

### Asyncronous Programming
```dart
void main() {
  // Asyncronous Programming
  // Future - 미래
  // 미래에 받아올 값
  Future<String> name = Future.value('이름');
  Future<int> number = Future.value(123);
  Future<bool> isTrue = Future.value(true);

  addNumbers(1, 1);
  addNumbers(2, 2);
}

void addNumbers(int number1, int number2) {
  print('계산 시작: $number1 + $number2');

  // 서버 시뮬레이션
  Future.delayed(Duration(seconds: 2), () {
    print('계산 완료: $number1 + $number2 = ${number1 + number2}');
  });

  print('함수 완료: $number1 + $number2');
}
```

### `async` & `await`
```dart
void main() {
  // `async` & `await`
  // Future - 미래
  // 미래에 받아올 값
  Future<String> name = Future.value('이름');
  Future<int> number = Future.value(123);
  Future<bool> isTrue = Future.value(true);

  addNumbers(1, 1);
  addNumbers(2, 2);
}

void addNumbers(int number1, int number2) async {
  print('계산 시작: $number1 + $number2');

  // 서버 시뮬레이션
  await Future.delayed(Duration(seconds: 2), () {
    print('계산 완료: $number1 + $number2 = ${number1 + number2}');
  });

  print('함수 완료: $number1 + $number2');
}
```
- `await` 키워드는 비동기 작업이 끝날 때까지 기다리게 해주는 기능을 합니다.
- `await`는 반드시 `Future`가 반환되는 함수에서 사용해야 합니다.
- `await`를 사용하려면, 그 코드를 `async` 함수 내에서 실행해야 합니다.

### `async` & `await`
```dart
void main() async {
  // `async` & `await`
  // Future - 미래
  // 미래에 받아올 값
  Future<String> name = Future.value('이름');
  Future<int> number = Future.value(123);
  Future<bool> isTrue = Future.value(true);

  await addNumbers(1, 1);
  await addNumbers(2, 2);
}

Future<void> addNumbers(int number1, int number2) async {
  print('계산 시작: $number1 + $number2');

  // 서버 시뮬레이션
  await Future.delayed(Duration(seconds: 2), () {
    print('계산 완료: $number1 + $number2 = ${number1 + number2}');
  });

  print('함수 완료: $number1 + $number2');
}
```

### `async` & `await`
```dart
void main() async {
  // `async` & `await`
  // Future - 미래
  // 미래에 받아올 값
  Future<String> name = Future.value('이름');
  Future<int> number = Future.value(123);
  Future<bool> isTrue = Future.value(true);

  int result1 = await addNumbers(1, 1);
  int result2 = await addNumbers(2, 2);

  print('result1: $result1');
  print('result2: $result2');
  print('result1 + result2 = ${result1 + result2}');
}

Future<int> addNumbers(int number1, int number2) async {
  print('계산 시작: $number1 + $number2');

  // 서버 시뮬레이션
  await Future.delayed(Duration(seconds: 2), () {
    print('계산 완료: $number1 + $number2 = ${number1 + number2}');
  });

  print('함수 완료: $number1 + $number2');

  return number1 + number2;
}
```

### Stream
```dart
import 'dart:async';

void main() {
  // Stream
  final streamController = StreamController();
  final stream = streamController.stream;

  final streamListener1 = stream.listen((value) {
    print('Listener 1: $value');
  });

  streamController.sink.add(1);
  streamController.sink.add(2);
  streamController.sink.add(3);
  streamController.sink.add(4);
  streamController.sink.add(5);
}
```
- `Future`를 사용하면 하나의 비동기 작업만 처리할 수 있지만, `Stream`은 여러 개의 비동기 작업을 하나의 스트림에서 처리할 수 있습니다.

### Broadcast stream
```dart
import 'dart:async';

void main() {
  // Broadcast stream
  final streamController = StreamController();
  final stream = streamController.stream.asBroadcastStream();

  final streamListener1 = stream.listen((value) {
    print('Listener 1: $value');
  });

  final streamListener2 = stream.listen((value) {
    print('Listener 2: $value');
  });

  streamController.sink.add(1);
  streamController.sink.add(2);
  streamController.sink.add(3);
  streamController.sink.add(4);
  streamController.sink.add(5);
}
```
- 기본적으로 `StreamController`는 단일 리스너만을 지원합니다. 즉, 스트림에 한 번에 하나의 리스너만 구독할 수 있습니다.
- 하지만 `asBroadcastStream()`을 사용하면 여러 리스너가 스트림을 동시에 구독할 수 있습니다. 이는 브로드캐스트 스트림이기 때문에 여러 리스너가 동시에 데이터를 받을 수 있게 해줍니다.

### Filtered stream
```dart
import 'dart:async';

void main() {
  // Filtered stream
  final streamController = StreamController();
  final stream = streamController.stream.asBroadcastStream();

  final streamListener1 = stream.where((value) => value % 2 == 0).listen((value) {
    print('Listener 1: $value');
  });

  final streamListener2 = stream.where((value) => value % 2 == 1).listen((value) {
    print('Listener 2: $value');
  });

  streamController.sink.add(1);
  streamController.sink.add(2);
  streamController.sink.add(3);
  streamController.sink.add(4);
  streamController.sink.add(5);
}
```
- `stream.where()`는 필터링을 통해 조건에 맞는 데이터만 통과시킵니다.
  - `streamListener1`은 짝수만 필터링하여 구독합니다.
  - `streamListener2`는 홀수만 필터링하여 구독합니다.
- 각 리스너는 자신이 구독한 스트림에서 조건에 맞는 값만 받게 됩니다.
- `where()`를 사용하면 스트림에서 특정 조건에 맞는 값만 필터링하여 구독할 수 있습니다.
- 필터링된 값만 리스너에게 전달되므로, 구독자가 자신이 필터링한 조건에 맞는 데이터만 받게 됩니다.
- 이로 인해 구독자1이 짝수만 구독하고 있다면 홀수는 전달되지 않으며, 구독자2는 홀수만 구독하므로 짝수는 전달되지 않습니다.

### Future function
```dart
import 'dart:async';

void main() async {
  // Future function
  final result = await calculate(5);

  print(result);
}

Future<int> calculate(int number) async {
  for (int i = 0; i < 5; i++) {
    return i * number;
  }

  return 0;
}
```
- `Future`는 한 번만 값을 반환할 수 있습니다.
- 위 코드에서 `return`이 호출되는 순간, 함수가 즉시 종료되며 남은 `for` 루프는 실행되지 않습니다.
- 따라서 `Future` 기반 비동기 함수는 한 번의 결과값을 비동기로 처리할 때 적합하지만, 여러 값을 순차적으로 반환하려면 한계가 있습니다.

### Stream function
```dart
import 'dart:async';

void main() {
  // Stream function
  calculate(5).listen((value) {
    print('$value');
  });
}

Stream<int> calculate(int number) async* {
  for (int i = 0; i < 5; i++) {
    yield i * number;
  }
}
```
- `Stream`은 데이터를 여러 번에 걸쳐 반환할 수 있습니다.
- `async*`와 `yield`를 사용하면 함수가 종료되지 않고, 반복적으로 값을 생성하고 스트림에 추가합니다.
- 이를 통해 구독자는 스트림에 추가되는 값을 실시간으로 받을 수 있습니다.
- `yield`는 값을 스트림에 추가하면서 함수의 실행 상태를 유지합니다. 다음 값을 생성할 때까지 대기 상태로 들어가며, 필요하면 비동기 작업도 수행할 수 있습니다.

### Future, stream function
```dart
import 'dart:async';

void main() {
  // Future, stream function
  calculate(5).listen((value) {
    print('$value');
  });

  calculate(7).listen((value) {
    print('$value');
  });
}

Stream<int> calculate(int number) async* {
  for (int i = 0; i < 5; i++) {
    yield i * number;

    await Future.delayed(Duration(seconds: 1));
  }
}
```

### `await` in `Future`, `yield*` in `Stream`
```dart
import 'dart:async';

void main() {
  // `await` in `Future`, `yield*` in `Stream`
  playAllStream().listen((value) {
    print(value);
  });
}

Stream<int> playAllStream() async* {
  yield* calculate(5);
  yield* calculate(7);
}

Stream<int> calculate(int number) async* {
  for (int i = 0; i < 5; i++) {
    yield i * number;

    await Future.delayed(Duration(seconds: 1));
  }
}
```
- `playAllStream` 함수는 두 개의 스트림을 순서대로 처리합니다.

### Record
```dart
void main() {
  // Record 사용 예제
  final result = nameAndAge({
    'name': '민지',
    'age': 20,
  });

  print(result);
  print(result.$1);
  print(result.$2);

  print('----------');

  // List에 Record를 활용한 예제
  final result2 = getNewJeansWithType();

  for (final item in result2) {
    print(item.$1);
    print(item.$2);
  }

  print('----------');

  // Named Record 사용 예제
  final result3 = getNewJeansWithType2();

  for (final item in result3) {
    print(item.$1);
    print(item.$2);
  }

  print('----------');

  // Named parameter 스타일의 Record 사용 예제
  final result4 = getNewJeansWithType3();

  for (final item in result4) {
    print(item.name);
    print(item.age);
  }

  print('----------');

  // 여러 필드를 포함한 Record 사용 예제
  final result5 = getMinji();

  print(result5);
  print(result5.$1);
  print(result5.$2);
  print(result5.$3);
}

// Record를 반환하는 함수
(String, int) nameAndAge(Map<String, dynamic> json) {
  return (json['name'] as String, json['age'] as int);
}

// Unnamed Record List를 반환하는 함수
List<(String, int)> getNewJeansWithType() {
  return [
    ('민지', 20),
    ('해린', 18),
  ];
}

// Named Record List를 반환하는 함수
List<(String name, int age)> getNewJeansWithType2() {
  return [
    ('민지', 20),
    ('해린', 18),
  ];
}

// Named parameter 스타일의 Record를 반환하는 함수
List<({String name, int age})> getNewJeansWithType3() {
  return [
    (name: '민지', age: 20),
    (name: '해린', age: 18),
  ];
}

// 여러 필드를 포함한 Record를 반환하는 함수
(String name, String group, int age) getMinji() {
  return ('민지', '뉴진스', 20);
}
```
- 타입과 순서를 보장: `(String, int)`처럼 고정된 타입과 순서를 제공하여 데이터 무결성을 유지합니다.
- 코드 간결성: 클래스를 정의하지 않아도 간단히 데이터 그룹을 표현할 수 있습니다.
- 가독성 향상: 데이터에 이름을 붙이거나(Named Record) 순서만 사용(Unnamed Record)하여 가독성을 높일 수 있습니다.
- List와 함께 사용하여 여러 Record를 관리할 수 있습니다.
- Named parameter 스타일 문법 `{}`을 사용하면 데이터 필드에 명확한 이름을 부여할 수 있습니다.

### Destructuring
```dart
void main() {
  // Destructuring(구조 분해 할당)
  final (name, age) = ('민지', 20); // Record의 데이터를 바로 변수에 할당할 수 있습니다.

  print(name);
  print(age);

  print('----------');

  final newJeans = ['민지', '해린'];

  final [a, b] = newJeans; // List의 데이터를 바로 변수에 할당할 수 있습니다.

  print(a);
  print(b);

  print('----------');

  final [String aa, String bb] = newJeans; // 타입을 지정하여 데이터를 할당할 수 있습니다.

  print(aa);
  print(bb);

  print('----------');

  final numbers = [1, 2, 3, 4, 5, 6, 7, 8];

  final [x, y, ..., z] =
      numbers; // Rest Matching은 List에서 나머지 데이터를 생략할 때 사용하며, 한 번만 사용할 수 있습니다.

  print(x);
  print(y);
  print(z);

  print('----------');

  final [xx, yy, ...rest, zz] =
      numbers; // Rest Matching에 이름을 지정하여 생략된 데이터를 별도로 사용할 수 있습니다.

  print(xx);
  print(yy);
  print(zz);
  print(rest);

  print('----------');

  final [xxx, _, yyy, ...rest2, zzz, _] =
      numbers; // `_`를 사용해 특정 데이터를 무시할 수 있습니다. 무시한 데이터는 별도로 사용할 수 없습니다.

  print(xxx);
  print(yyy);
  print(zzz);
  print(rest2);

  print('----------');

  final minJiMap = {
    'name': '민지',
    'age': 20,
  };

  final {
    // Map을 Destructuring할 경우, key와 매칭되는 변수 이름을 명시해야 합니다.
    'name': name2,
    'age': age2,
  } = minJiMap;

  print(name2);
  print(age2);

  print('----------');

  final minJiIdol = Idol(name: '민지', age: 20);

  final Idol(name: name3, age: age3) =
      minJiIdol; // Class도 Destructuring이 가능합니다. Dart에서는 대부분의 데이터 구조에서 Destructuring을 지원합니다.

  print(name3);
  print(age3);
}

class Idol {
  final String name;
  final int age;

  Idol({
    required this.name,
    required this.age,
  });
}
```

### Pattern Matching
```dart
void main() {
  switcher('aaa');
  switcher(['1', '2']);
  switcher([1, 2, 3]);
  switcher([4, 5, 6]);
  switcher([7, 8]);
  switcher(8);
  switcher(15);

  print('----------');

  print(switcher2(8, true));
  print(switcher2(15, true));
  print(switcher2(15, false));

  print('----------');

  forMatcher();

  print('----------');

  ifMatcher();
}

// Dart의 switch에서 패턴 매칭을 사용할 수 있습니다.
// 각 case에 다양한 패턴(문자열, 리스트, 조건)을 적용할 수 있습니다.
void switcher(dynamic anything) {
  switch (anything) {
    case 'aaa':
      print('match: aaa');
      break;
    case ['1', '2']:
      print('match: [1, 2]');
      break;
    case [_, _, _]:
      print('match: [_, _, _]');
      break;
    case [int a, int b]:
      print('match: [int $a, int $b]');
      break;
    case > 5 && < 10:
      print('match: > 5 && < 10');
      break;
    default:
      print('no match');
      break;
  }
}

// switch 내부에서 arrow function을 사용해 각 case에 해당하는 값을 반환할 수 있습니다.
// when 키워드를 사용하면 조건부로 특정 case를 매칭할 수 있습니다.
String switcher2(dynamic anything, bool condition) => switch (anything) {
      8 => 'match: 8',
      15 when condition => 'match: 15 && true',
      _ => 'no match',
    };

void forMatcher() {
  final List<Map<String, dynamic>> members = [
    {
      'name': '민지',
      'age': 20,
    },
    {
      'name': '해린',
      'age': 18,
    },
  ];

  for (final member in members) {
    // 패턴 매칭을 사용하지 않는 기존 방식
    print(member['name']);
    print(member['age']);
  }

  print('----------');

  for (final {'name': name, 'age': age} in members) {
    // for 안에서도 pattern matching(destructuring)을 사용할 수 있습니다.
    print(name);
    print(age);
  }
}

void ifMatcher() {
  final member = {
    'name': '민지',
    'age': 20,
  };

  // member가 지정된 패턴과 매칭되면(조건을 만족하면) 해당 내용을 실행합니다.
  // 이와 같이 if 문에서도 패턴 매칭을 사용할 수 있습니다.
  if (member case {'name': String name, 'age': int age}) {
    print(name);
    print(age);
  }
}
```

