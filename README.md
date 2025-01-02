# Dart

### Hello, World! 출력
```dart
void main() {
  print('Hello, World!');
}
```

### 변수 사용
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

### 정수형 변수 사용
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

### 정수형 변수 연산
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

### 실수형 변수 연산
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

### 불리언 변수 사용
```dart
void main() {
  // boolean
  bool isTrue = true;
  bool isFalse = false;

  print(isTrue);
  print(isFalse);
}
```

### 문자열 및 타입 확인
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

### 문자열 결합 및 문자열 내 변수 삽입
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

### 동적 타입 변수 사용 및 타입 변경
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

### 널 허용 및 널 불허 변수 사용
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

### final과 const를 이용한 값 할당
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

### final과 const를 이용한 변수 선언
```dart
void main() {
  // final, const
  final message1 = 'Hello, World!';

  print(message1);

  const message2 = 'Hello, New World!';

  print(message2);
}
```

### 산술 연산자 사용
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

### 증감 연산자 및 복합 대입 연산자 사용
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

### 널 병합 할당 연산자 사용
```dart
void main() {
  // null
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

### 비교 연산자 사용
```dart
void main() {
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

### 타입 검사 연산자 사용
```dart
void main() {
  int number = 1;

  print(number is int);
  print(number is String);

  print(number is! int);
  print(number is! String);
}
```

### 논리 연산자 사용
```dart
void main() {
  // &&(AND), ||(OR)
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

### 리스트 사용 및 인덱싱
```dart
void main() {
  // List
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

### 리스트 수정 및 메서드 사용
```dart
void main() {
  // List
  List<String> alphabet = ['a', 'b', 'c', 'd', 'e'];
  
  print(alphabet.length);
  
  alphabet.add('f');
  
  print(alphabet);
  
  alphabet.remove('f');
  
  print(alphabet);
  
  print(alphabet.indexOf('c'));
}
```

### 맵 사용 및 수정
```dart
void main() {
  // Map
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

### 셋 사용 및 수정
```dart
void main() {
  // Set
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

### if-else 조건문 사용
```dart
void main() {
  // if
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

### switch-case 조건문 사용
```dart
void main() {
  // switch
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

### for 루프 및 for-in 루프 사용
```dart
void main() {
  // for loop
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

### while 루프 및 do-while 루프 사용
```dart
void main() {
  // while loop
  int i = 0;

  while (i < 10) {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  }

  i = 0;

  // do while loop
  do {
    print(i);
    i++;

    if (i == 5) {
      break;
    }
  } while (i < 10);
}
```

### break 및 continue 제어문 사용
```dart
void main() {
  // break
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      break;
    }

    print(i);
  }

  // continue
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      continue;
    }

    print(i);
  }
}
```

### enum 사용
```dart
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

### 순서 있는 매개변수를 사용하는 함수 정의
```dart
void main() {
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

### 선택적 매개변수를 사용하는 함수 정의
```dart
void main() {
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

### 이름 있는 매개변수를 사용하는 함수 정의
```dart
void main() {
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

### 필수 및 선택적 이름 있는 매개변수를 사용하는 함수 정의
```dart
void main() {
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

### 매개변수를 혼합하여 사용하는 함수 정의
```dart
void main() {
  int result1 = add(10, y: 20);
  int result2 = add(1, y: 3, z: 5);

  print('result1: $result1');
  print('result2: $result2');
  print('result1 + result2: ${result1 + result2}');
}

// 3개의 수(x, y, z)를 덧셈한 결과가 짝수인지 홀수인지 알려주는 함수
// parameter(argument): 매개변수
// positio용
```dart
void main() {
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

### 함수 타입을 이용한 연산
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
