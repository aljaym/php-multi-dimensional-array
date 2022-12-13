# Workingg with multi dimensional array in php 

To use updateInventory.

If product is new and not yet existing in 1st array simply add it and if item is already in 1st array you'll just need to update the inventory count in 1st array 0 index.

eg.
```php
// Example inventory lists
$curInv = [
    [21, "Bowling Ball"],
    [2, "Dirty Sock"],
    [1, "Hair Pin"],
    [5, "Microphone"]
];

$newInv = [
    [2, "Hair Pin"],
    [3, "Half-Eaten Apple"],
    [67, "Bowling Ball"],
    [7, "Toothpaste"]
];

print_r(updateInventory($curInv, $newInv));
```
