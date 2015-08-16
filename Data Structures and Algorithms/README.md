#JavaScript Arrays Defined

- linear collection of elements where elements can be accessed via indeces.
- javascript arrays are just objects they are not quite as efficient as the arrays of other programming languages.

### Creating arrays

```
var numbers = [];
// numbers.length   displays 0

var numbers = [1, 2, 3, 4, 5];
// numbers.length  - dosplays 5

var numbers = new Array(); // calling the array constructor
// numbers.length  - displays 0

var numbers = new Array(1,2,3,4,5);
// numbers.length  - dosplays 5

var numbers = new Array(10); // single argument specifying the length of the array
// numbers.length  - dosplays 10

// javascript array elements do not all have to be of the same type
var objects = [1, "joe", true, null];


// to verify object is an array
Array.isArray(objects);

```
### Accessing and writing array elements
- use [] operator
- use for loops

### Creating Arrays from Strings
```
var sentence = "the quick brown fox jumped over the lazy dog" ;
var words = sentence. split(" " );

```
### Aggregate Array Operations
- assign one array to another 
	- when you assign one array to another array, you are assigning a reference to the assigned array.
	 ```
	 var nums = [];
	 for (var i = 0; i<200; ++i  ){
	 	nums[i] =  i+1;
	 }
	 var samenums = nums;
	 nums[0] = 400;
	 console.log(samenums[0]);
	 ```
- this is called SHALLOW COPY 

## Accessor Functions
### Searching for a value
```
var names = ["David" , "Cynthia" , "Raymond" , "Clayton" , "Jennifer" ];
var position = names.indexOf("Clayton");
if (position >= 0) {
	console.log('found');
}else{
	console.log("not found");
}
```
