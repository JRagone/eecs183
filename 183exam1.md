Exam 1 Notecard Topics
======================

## Functions

``` cpp
return_type function_name( parameters )
{
	/* Some code */
	return object_of_return_type;
}
```

First line is function's declaration: the function's name, return type, and parameters.

## Array Traversal

The following traverses every element in an array by index

``` cpp
for ( int i = 0; i < array_length; i++ ) {
	/* do something with arr[i], for example */
}
```

### Example

Need to print every element divisible by 4? Use the modulo operator `%`

``` cpp
for ( int i = 0; i < array_length; i++ ) {
	if ( my_arr_of_nums[i] % 4 == 0 ) {
		cout << "The quotient of this value and 4 has remainder 0: " << my_arr_of_nums[i] << endl;
	}
}
```

## Testing

Test edge cases! Look at the RME to see if your code succeeds with the minimal requirement, and think of ways you could break it while following the RME.

Don't worry about handling input that doesn't follow the RME

## `iostream`

``` cpp
cin >>
cout <<
```

`cin` is used with the extraction operator `>>`

Every time you call `cin >>`, the program will read input from the stream up to the next instance of whitespace.

`cout` is used with the insertion operator `<<`

## Pass-by-reference `&`

``` cpp
void add_five(int & input) {
	input += 5;
}

int main( ) {
	int num = 0;
	cout << "Original value: " << num << endl; // Original value: 0
	add_five(num);
	cout << "New value: " << num << endl; // New value: 5;
}
```

In the context of parameters, for example, `&` is the pass-by-reference modifier. This modifier enables you to modify the value of the parameter, rather than modifying the value of a copy of the parameter, which is the case when `&` is not used.

## Operations

`x/y` will always truncate the quotient if two numbers do not divide cleanly, i.e. 5/3 = 1 (.6666 is truncated)

`x%y` will return the remainder of `x/y`

## ASCII

How to check that a character is between a and z?

``` cpp
if ( letter >= 'a' && letter <= 'z' ) {
	cout << "It's in between!" << endl;
}
```

Note that this is possible thanks to [ASCII](https://en.wikipedia.org/wiki/ASCII). Think of every character as representing a number and know that your intuition is correct that `a < z` or `A < Z`

## Loops

The for-loop syntax contains three expressions corresponding to the three components ofany loop, which are: ​**initialization**​,  ​**test**​ and ​**update**

## Datatypes

`int`, `double`, `char`, etc.

### Casting

Converting the ​`double`​ value of a variable into an ​`int`​ value and viceversa is known as **casting**

