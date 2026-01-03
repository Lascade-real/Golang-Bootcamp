package basics

import (
	"fmt"
	"math"
)

func main() {
	//variables delcaration
	var a, b int = 10, 3 //13
	var c, d int = 11, 8 //3
	var e, f int = 12, 9 //108
	var g, h int = 10, 3 //1
	var result int

	result = a + b
	fmt.Println("Add: ", result)

	result = c - d
	fmt.Println("Subtract: ", result)

	result = e * f
	fmt.Println("Multiple: ", result)

	result = g / h
	fmt.Println("Division: ", result)

	result = g % h
	fmt.Println("Division: ", result)

	const p float64 = 22.0 / 7
	fmt.Println(p)

	//Overflow with Signed Integer
	var maxInt int64 = 9223372036854775807 //max value that int64 can hold
	fmt.Println(maxInt)

	maxInt = maxInt + 1
	fmt.Println(maxInt)

	//Overflow with Unsigned Integer
	var uMaxInt uint64 = 18446744073709551615 //max value for uint64 type
	fmt.Println(uMaxInt)

	uMaxInt = uMaxInt + 1
	fmt.Println(uMaxInt)

	//Underflow with small float
	var smallFloat float64 = 1.0e-323
	fmt.Println(smallFloat)

	smallFloat = smallFloat / math.MaxFloat64
	fmt.Println(smallFloat)

}
