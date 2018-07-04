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
