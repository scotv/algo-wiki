# Sorting
In our sorting, we pass a function as parameters, named `compare(x, y) : number`. We sort the array by comparing each two value resulted from `x`, where `x`is an element of array.

The default `compare(x, y) : number` is `(x, y) => x - y`. While, we can pass `(x, y) => y -x` to order by DESC, or we can pass `(x, y) => y^2 - x^2` to order by DESC of each absolute value.

<a name="static" />
## Static
|| *Call* || *Meaning* ||
|| `isSorted(arr, compare): boolean` || gets a boolean value indicating whether arr is sorted under comparing rule for `item` ||
|| `quickSort(arr, compare): []` || gets a new sorted array by quick sort ||
|| `mergeSort(arr, compare): []` || gets a new sorted array by merge sort ||
|| `mergeSortBU(arr, compare): []` || gets a new sorted array by bottom-up merge sort ||
|| `heapSort(arr, option): []` || gets a new sorted array by heap sort, `option == {order:'ASC' | 'DESC'}`||