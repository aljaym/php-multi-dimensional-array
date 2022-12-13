# To use updateInventoryTest.php

If product not yet existing in current inventory array simply add it and if item is already in current inventory array you'll just need to update the qty count in 1st array 0 index.

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

Sample Result
```php
Array
(
    [0] => Array
        (
            [0] => 88
            [1] => Bowling Ball
        )

    [1] => Array
        (
            [0] => 2
            [1] => Dirty Sock
        )

    [2] => Array
        (
            [0] => 3
            [1] => Hair Pin
        )

    [3] => Array
        (
            [0] => 5
            [1] => Microphone
        )

    [4] => Array
        (
            [0] => 3
            [1] => Half-Eaten Apple
        )

    [5] => Array
        (
            [0] => 7
            [1] => Toothpaste
        )

)
```
