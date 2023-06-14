
### Array vs Slice

#### Array
    var array [5]string // you define length
    array[1] = "2"
    fmt.Println(array)
<br/> 

#### Slice
	var slice []string // you don't define lenght
    slice = append(slice, 1) // to add new itens you should have use the append only
    fmt.Println(slice)
    
    //Another way

    array := [5]int{1, 2, 3, 4, 5}
	fmt.Println(array)

	slice := array[1:3] // The slice is the poiter of array
	fmt.Println(slice)
	
	array[1] = 99 // You change the array
	fmt.Println(slice) // Slice value changes as well