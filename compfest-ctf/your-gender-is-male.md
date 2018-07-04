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

