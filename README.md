# best regular expression for gmail
Gmail Regular expression with all details (not start with dot,number , is it possible to use multiple dot but not in a row and so on)


# Gmail regular expression (Full version)

In this mini project I'm going to introduce great pattern or regular expression for GMAIL input and validating them every where that you want.


## Usage in PHP

```php
dd(preg_match('/^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com/', 'ali.rezvaniara@gmail.com'))
# returns 1/true

dd(preg_match('/^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com/', 'ali..rezvaniara@gmail.com'))
# returns 0/false

dd(preg_match('/^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com/', '2ali.rezvaniara@gmail.com'))
# returns 0/false


dd(preg_match('/^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com/', 'ali2.rezvaniara@gmail.com'))
# returns 1/true

dd(preg_match('/^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com/', '.ali.rezvaniara@gmail.com'))
# returns 0/false

```


## Usage in HTML

```html
<!DOCTYPE html>
<html>
<body>

<h1>Example using of GMAIL regular expression in html</h1>

<form action="/action_page.php">
  <input type="text" id="email" name="email" pattern="^[^0-9^.][a-zA-Z0-9]+(\.?[a-z]+)*@gmail.com" >
  <input type="submit">
</form>

<p><strong>Note:</strong> The pattern attribute of the input is not supported in Safari 10 (or earlier).</p>

</body>
</html>


```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
