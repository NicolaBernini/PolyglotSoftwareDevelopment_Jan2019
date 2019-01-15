
# Overview 

Maps or Dictionaries essentially allow to define Key-Values Unique Associations 

# Interface 

Maps interface typically include the following operations 
- Requiring `key` and `value` 
  - Definition 
  - Insert

- Requiring `key` 
  - Lookup
  - Modify 
  - Delete 



# Languages 

| Operation     | Definition (Homogeneous Type) | Definition (Heterogeneous Type)  | Lookup |
| ------------- | ------------- | ----- | --- |
| Python    | `a = {'key': 'value'} ` | `a = {'key': 'value', 1: 'test', 'mytest': 6} ` | `a['key'], a[1]`  |
| Scala    | `var a = ("key" -> "value") ` | `var a = ("key" -> "value", 1 -> "test", "mytest" -> 6) ` | `a("key"), a(1)`  |
| Javascript    | `a = {'key': 'value'} ` | `var a = {'key': 'value', 1: 'test', 'mytest': 6} ` | `a['key'], a[1]`  |
| C++14    | `map<string, string> a = {{"key", "value"}}; ` | Not standard | `a["key"]`  |


# Comments 

## About C++ 

C++ is a statically typed language, which means you have to fix what are the `Key Type` and the `Value Type` at declaration time and they remain fixed hence type mixing results in a violation of this constraints and raises a compilation error

However historically we had out of standard solutions like [`boost::variant`](https://www.boost.org/doc/libs/1_64_0/doc/html/variant.html) and since C++17 this element has been standardized in [`std::variant`](https://en.cppreference.com/w/cpp/utility/variant) 




