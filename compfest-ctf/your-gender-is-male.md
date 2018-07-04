write up "your gender is male" COMPFEST CTF 2018
------------------------------------------------

```
<?php
  include 'flag.php';
  if (isset($_POST['guess'])) {
    extract($_POST);
    if ($guess == $number) {
      die($flag);
    }
  }
?>
```

clue:
-----
```
You solve this problem as a Man. Man is always wrong, woman is always right.
```

snippets of `extract` function from php5.net

```
<?php

/* Suppose that $var_array is an array returned from
 *    wddx_deserialize */

$size = "large";

$var_array = array("color" => "blue",
                   "size"  => "medium",
                   "shape" => "sphere");

extract($var_array, EXTR_PREFIX_SAME, "wddx");

echo "$wddx_color, $size, $shape, $wddx_size\n";

?>

```

another snippets:

```
<!DOCTYPE html>
<html>
<body>

<?php

$a = "Original";

$my_array = array("a" => "Cat","b" => "Dog", "c" => "Horse");

echo($a);

extract($my_array);

echo "\$a = $a; \$b = $b; \$c = $c";

?>

</body>
</html>

```
