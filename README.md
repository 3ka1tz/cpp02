# CPP Module 02
Ad-hoc polymorphism, operator overloading and the [Orthodox Canonical class form](https://riceset.com/C++/The-Orthodox-Canonical-Class-Form).

## [Exercise 00: My First Class in Orthodox Canonical Form](https://github.com/3ka1tz/cpp02/tree/main/project/ex00)
Create a class in Orthodox Canonical Form that represents a fixed-point number:

- Public members:
  - A default constructor that initializes the fixed-point number value to 0.
  - A copy constructor.
  - A copy assignment operator overload.
  - A destructor.
  - A member function `int getRawBits() const;` that returns the raw value of the fixed-point value.
  - A member function `void setRawBits(int const raw);` that sets the raw value of the fixed-point number.

- Private members:
  - An integer to store the fixed-point number value.
  - A static constant integer to store the number of fractional bits. Its value will always be the integer literal 8.

## [Exercise 01: Towards a more useful fixed-point number class](https://github.com/3ka1tz/cpp02/tree/main/project/ex01)
The previous exercise was a good start, but our class is pretty useless. It can only represent the value 0.0.

Add the following public constructors and public member functions to your class:

- A constructor that takes a constant integer as a parameter.
It converts it to the corresponding fixed-point value. The fractional bits value
should be initialized to 8, like in exercise 00.

- A constructor that takes a constant floating-point number as a parameter.
It converts it to the corresponding fixed-point value. The fractional bits value
should be initialized to 8, like in exercise 00.

- A member function float toFloat( void ) const;
that converts the fixed-point value to a floating-point value.

- A member function int toInt( void ) const;
that converts the fixed-point value to an integer value.

And add the following function to the Fixed class files:
- An overload of the insertion («) operator that inserts a floating-point representation
of the fixed-point number into the output stream object passed as a parameter.

## [Exercise 02: Now we’re talking](https://github.com/3ka1tz/cpp02/tree/main/project/ex02)


### Personal Recommendations
