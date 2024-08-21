# Lists vs Maps

## Lists in Dart
A List in Dart is an ordered collection of elements that can be of any type. It allows you to store multiple items in a single variable and access them by their index. Lists are zero-based, meaning the first element is at index 0.

### Syntax:
**Creating an empty list:**
```
var list = [];

or with explicit type:

List<int> list = [];
```

**Creating a list with initial values:**
```
var list = [1, 2, 3, 4, 5];

or with explicit type:

List<String> list = ['apple', 'banana', 'cherry'];
```
## Common Operations in List:

### Accessing elements:
`var firstElement = list[0]; // Gets the first element`

### Adding elements:
`list.add(6); // Adds an element at the end`

### Inserting elements:
`list.insert(1, 10); // Inserts 10 at index 1`
### Removing elements:
`list.remove(2); // Removes the first occurrence of 2`

### Iterating:
```
for (var item in list) {
  print(item);
}
```

### Use Cases
- Storing ordered data, such as a list of items in a shopping cart.
- Iterating through elements when order matters.

## Maps in Dart
A Map in Dart is a collection of key-value pairs. Each key in a map is unique, and each key maps to exactly one value. Maps are also known as dictionaries or hash tables in other languages.

### Syntax:

**Creating an empty map:**
```
var map = <String, dynamic>{};
or with type inference:
var map = {};
```

**Creating a map with initial values:**
```
var map = {
  'name': 'John',
  'age': 30,
  'city': 'New York'
};
```

## Common Operations in Maps:

### Accessing values:
`var name = map['name']; // Gets the value for the key 'name'`

### Adding/Updating entries:
map['occupation'] = 'Developer'; // Adds or updates the 'occupation' key

### Removing entries:
`map.remove('city'); // Removes the entry with key 'city'`

### Iterating:
```
map.forEach((key, value) {
  print('$key: $value');
});
```
### Use Cases:
- Storing data where you need to quickly look up values based on unique keys.
- Representing configurations, settings, or any data where each value is associated with a specific key.

## Summary
## Lists
- **Definition:** Ordered collection of elements.
- **Access:** By index.
- **Common Use:** Storing sequences of items.
  
Lists in Dart are ordered collections of elements that can be accessed by their index. You can create a list with initial values or start with an empty list and add elements later. Lists are useful when you need to maintain an ordered sequence of items, such as user input or a collection of records.

## Maps
- **Definition:** Collection of key-value pairs.
- **Access:** By key.
- **Common Use:** Associating values with unique keys for quick lookups.

Maps in Dart store data as key-value pairs where each key is unique and maps to a specific value. You can create a map with predefined keys and values or start with an empty map and add entries as needed. Maps are ideal for situations where you need to retrieve data based on a unique identifier, such as user settings or configuration options.
