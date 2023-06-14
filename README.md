
### Array vs Slice
Basically in **Array** you define the length, however **Slice** is not necessary.
In **Go** is not common people use arrays because the length defined. **Slice** are **more flexible**.

Defining
````go
var array [5]int //defined length
var slice []int // not defined
````

Adding
````go
array[0] = 1
array[1] = 2
array[2] = 3
array[3] = 4
array[4] = 5

slice = append(slice, 1, 2, 3, 4, 5)
````

Initializing
````go

var array = [5]int{1,2,3,4,5}
var slice2 = []int{1, 2, 3, 4, 5}

array := [5]int{1, 2, 3, 4, 5}
array2 := [...]int{1,2,3,4,5}

slice2 := []int{1, 2, 3, 4, 5}
````

````go
var slice []string // you don't define lenght
slice = append(slice, 1) // to add new itens you should have use the append only
fmt.Println(slice)
    
//Another way
array := [5]int{1, 2, 3, 4, 5}
fmt.Println(array)


// Look this:
slice := array[1:3] //The slice is the poiter of array
fmt.Println(slice)
	
array[1] = 99 // You change the array
fmt.Println(slice) // Slice value changes as well
````