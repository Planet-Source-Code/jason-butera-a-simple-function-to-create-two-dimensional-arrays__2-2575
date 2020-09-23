<div align="center">

## A simple function to create two\-dimensional arrays


</div>

### Description

A lot of people have posts on Google asking how to create multidimensional arrays in Javascript. This function is easy to call and will create both one and two dimensional arrays. Please vote if you find that this code saves you time in your array coding. Thanks!
 
### More Info
 
First Argument: The first dimension of the array

Second Argument (Optional): The second dimension of the array

An array object with the specified dimensions.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jason Butera](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jason-butera.md)
**Level**          |Intermediate
**User Rating**    |4.8 (24 globes from 5 users)
**Compatibility**  |
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__2-67.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jason-butera-a-simple-function-to-create-two-dimensional-arrays__2-2575/archive/master.zip)





### Source Code

```
<SCRIPT LANGUAGE="JavaScript">
function CreateArray(dim1) {
	if (CreateArray.arguments.length == 1) {
		return new Array(dim1);
	} else {
		var multiArray = new Array(dim1)
		for (var i = 0; i < dim1; i++) {
			multiArray[i] = new Array(CreateArray.arguments[1]);
		}
		return multiArray;
	}
}
//Create a one-dimensional array
var myArray = CreateArray(5);
//Create a two-dimensional array
var myArray = CreateArray(5,2);
//Looping through the two-dimensional array
for (var i = 0; i <= myArray.length-1; i++) {
	for (var j = 0; j < myArray[i].length; j++) {
		// alert(myArray[i][j]);
	}
}
</SCRIPT>
```

