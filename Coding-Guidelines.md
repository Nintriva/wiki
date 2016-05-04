# Coding Guidelines
All code must conform to the guidelines outlined in this document. This allows for consistency and enables teams to function more efficiently when working on the same codebase.

## 1. Naming Conventions

#### Class & Function Names
1. Use `CamelCase` for all class and function names.
  ```
    class MyFirstClass{
    ...
    }
    // good

    class myfirstClass{
    ...
    }
    // bad


    public function MyFirstFunction{
    ...
    }
    // good

    public function myfirstFunction{
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
Ideally, code should be self documenting. Writing clear, concise, single function methods work better than bloated complex methods which perform several different tasks. See [Code Style](#3-code-style) for more information.

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
    ...
    }
    // good

    public function GetLargestPrimeFactor($number){
    ...
    }
  ```

## 3. Code Style

## 4. File Names

## 5. References

- [Python PEP Coding Guidelines](https://www.python.org/dev/peps/pep-0008/)
- [PSR 2 Coding Guidelines](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md)
- [PSR 1 Coding Guidelines](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md)

