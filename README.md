### Dart Language Fundamentals

#### Variables

Variables in Dart are like containers where you store data. You can declare them in a few different ways depending on your needs.

1. **`var` keyword**: When you use `var`, Dart will automatically figure out the type of the variable from the value you assign to it.
2. **`final` keyword**: A `final` variable can only be set once. Once you assign it a value, you can't change it.
3. **`const` keyword**: A `const` variable is a compile-time constant. This means its value is fixed when the program is compiled and cannot be changed afterward.

Here’s a simple example:

```dart
void main() {
  var name = 'John';       // Dart understands this is a String
  final age = 30;          // Dart understands this is an int, and you can't change it
  const pi = 3.14159;      // This is a constant value

  print('Name: $name');
  print('Age: $age');
  print('Pi: $pi');
}
```

#### Data Types

Dart is a statically-typed language, meaning every variable has a specific type that does not change. Here are some common data types:

1. **Numbers**: `int` for whole numbers and `double` for decimal numbers.
2. **Strings**: Represented by the `String` type, these are sequences of characters.
3. **Booleans**: The `bool` type has only two values: `true` or `false`.
4. **Lists**: A collection of items, represented by `List`.
5. **Maps**: A collection of key-value pairs, represented by `Map`.
6. **Sets**: A collection of unique items, represented by `Set`.

Here’s how you might use these data types:

```dart
void main() {
  int a = 10;                // Whole number
  double b = 3.14;           // Decimal number
  String c = 'Hello Dart';   // Sequence of characters
  bool isTrue = true;        // Boolean value
  List<int> numbers = [1, 2, 3];  // List of integers
  Map<String, int> ages = {'Alice': 25, 'Bob': 30};  // Map with string keys and int values
  Set<String> fruits = {'Apple', 'Banana', 'Cherry'};  // Set of unique strings

  print(a);
  print(b);
  print(c);
  print(isTrue);
  print(numbers);
  print(ages);
  print(fruits);
}
```

#### Operators

Dart has different operators to perform operations on variables and values.

1. **Arithmetic Operators**: These include `+` (addition), `-` (subtraction), `*` (multiplication), `/` (division), and `%` (modulus).
2. **Equality and Relational Operators**: These include `==` (equal), `!=` (not equal), `>` (greater than), `<` (less than), `>=` (greater than or equal to), and `<=` (less than or equal to).
3. **Logical Operators**: These include `&&` (logical AND), `||` (logical OR), and `!` (logical NOT).
4. **Assignment Operators**: These include `=` (assign), `+=` (add and assign), `-=` (subtract and assign), `*=` (multiply and assign), `/=` (divide and assign), and `%=` (modulus and assign).
5. **Conditional Operators**: These include `?:` (ternary operator) and `??` (if null operator).

Here are some examples:

```dart
void main() {
  // Arithmetic Operators
  int x = 5;
  int y = 2;
  print('x + y = ${x + y}'); // Adds x and y
  print('x - y = ${x - y}'); // Subtracts y from x
  print('x * y = ${x * y}'); // Multiplies x by y
  print('x / y = ${x / y}'); // Divides x by y
  print('x % y = ${x % y}'); // Remainder of x divided by y

  // Equality and Relational Operators
  print('x == y: ${x == y}'); // Checks if x is equal to y
  print('x != y: ${x != y}'); // Checks if x is not equal to y
  print('x > y: ${x > y}');   // Checks if x is greater than y
  print('x < y: ${x < y}');   // Checks if x is less than y
  print('x >= y: ${x >= y}'); // Checks if x is greater than or equal to y
  print('x <= y: ${x <= y}'); // Checks if x is less than or equal to y

  // Logical Operators
  bool a = true;
  bool b = false;
  print('a && b: ${a && b}'); // Logical AND
  print('a || b: ${a || b}'); // Logical OR
  print('!a: ${!a}');         // Logical NOT

  // Assignment Operators
  int z = 10;
  z += 5;  // Adds 5 to z
  print('z += 5: $z'); // z is now 15

  // Conditional Operators
  int? nullableValue;
  int nonNullableValue = nullableValue ?? 100; // If nullableValue is null, use 100
  print('nonNullableValue: $nonNullableValue'); // Prints 100
}
```

### In Short

- **Variables**: Use `var` to let Dart infer the type, `final` for variables that can only be set once, and `const` for compile-time constants.
- **Data Types**: Include `int`, `double`, `String`, `bool`, `List`, `Map`, and `Set`.
- **Operators**: Arithmetic, equality, relational, logical, assignment, and conditional operators help you perform various operations on your data.

Understanding these basics will help you get started with Dart and build more complex programs.
