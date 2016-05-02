# Coding Guidelines
All code must conform to the guidelines outlined in this document. This allows for consistency and enables teams to function more efficiently when working on the same codebase.

## 1. Naming Conventions

#### Class & Function Names
1. Use `CamelCase` for all class and function names.
  ```
    public function MyFirstClass{
    ...
    }
    // good

    public function myfirstClass{
    ...
    }
    // bad
  ```

#### Variables
1. Use descriptive names for variables except where convention states otherwise (e.g. loop variable names).
  ```
    $counter = 1;
    // good

    $c = 1;
    // bad

    for ($x = 1; $x < 5; $x++){
    ...
    }
    // good
  ```
2. Variable names must be `lowercase`.
3. Multi word variable names must be `separated_by_an_underscore`.

  ```
    $string = "string";
    // good
    $a_string = "a string";
    // good

    $String = "string";
    // bad
    $someString = "some string";
    // bad
  ```

#### Constants
1. Constants should be `CAPITALISED` and for multi-word constant names `SEPARATED_BY_UNDERSCORES`.
  ```
    STATUS_ACTIVE = 1;
    // good

    statusActive = 1;
    // bad
  ```

## 2. Documentation

#### Classes & Functions
1. Use [JavaDoc](http://www.oracle.com/technetwork/articles/java/index-137868.html), [PHPDoc](https://www.phpdoc.org/docs/latest/index.html) or [jsDoc](http://usejsdoc.org/about-getting-started.html) where appropriate. All three are very similar in structure with a few exceptions.

2. All functions should have documentation meta data unless the function is sufficiently simple and the name is self explanatory.
  ```
    /**
    * This function finds the largest prime factor of any given integer
    * @param integer $number The number for which the largest prime factor should be found
    * @return integer The largest prime factor of $number
    **/
    public function FindLargestPrimeFactor($number){
    }
    // good
  ```

## 3. File Names

## 4. References

- [Python PEP Coding Guidelines](https://www.python.org/dev/peps/pep-0008/)

