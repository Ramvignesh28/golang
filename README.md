package main
import "fmt"
func main() {
	numbers := [] int{1,2,3,4,5,6,7,8,9,10,11,12,19,15}
	fmt.Printf("numbers: %v\n", numbers)
	fmt.Printf("length: %v\n", len(numbers))
	fmt.Printf("capacity: %v\n", cap(numbers))
	//copy
	neededNumbers := numbers[: len(numbers)-10]
	numbersCopy := ([] int(neededNumbers))
	copy(numbersCopy, neededNumbers)
	fmt.Printf("numbersCopy: %v\n", numbersCopy)
	fmt.Printf("length: %v\n", len(numbersCopy))
	fmt.Printf("capacity: %v\n", cap(numbersCopy))
	
}
