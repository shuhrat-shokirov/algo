##1. Search function to check if the value is in the list.
###### Strictly so that the list is sorted !!!!
###### Otherwise, this function does not work !!!!

```
func main() {
	var (
		a      = DataInt{}
		search = NewBinSearch()
		b      = DataStr{}
	)
	a.List = []int{1, 2, 3, 4}
	a.Data = 6
	result := search.CheckDataInt(0, len(a.List)-1, a)
	fmt.Println(result)

	b.List = []string{"A", "B", "E", "F"}
	b.Data = "A"
	result = search.CheckDataStr(0, len(b.List)-1, b)
	fmt.Println(result)
}
```