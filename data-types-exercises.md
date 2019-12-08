### Assorted Data Types

#### What are the outputs and/or side effects of the following code snippets?

* Make a guess before testing your answer.
* "Error out" is a valid answer choice.
* Also include a sentence on why you chose your answer.

```rb
2 ** 3


```
```8
```

```rb
((16 / 4) * (2 + 1)) ** 2
```
```144
```

```rb
("a milli " + "a milli") * 3
```
```a milli a millia milli a millia milli a milli
```

```rb
("a milli " * 4) / 2
```
```(NoMethodError)
```

```rb
my_favorite_number = 13
puts "My favorite number is: " + my_favorite_number
```
```Error.
```

```rb
my_favorite_number = 13
puts "My favorite number is: #{my_favorite_number}"
```
```My favorite number is: 13
```

### Truthiness and Falsiness

#### Which of these evaluate as `false` in Ruby? Mark all that apply.

```text
[ ] false
[ ] 0
[ ] ""
[ ] null
[ ] [ ] (empty array)
[ ] undefined
[ ] NaN
[ ] nil
```
[ ] false
[ ] nil
#### What are the outputs and/or side effects of the following code snippets?

* Make a guess before testing your answer.
* "Error out" is a valid answer choice.
* Also include a sentence on why you chose your answer.

```rb
no_name = ""
if no_name
  puts "My name is: " + no_name
end
```
```My name is: 
```

```rb
no_name = nil
if no_name
  puts "My name is: " + no_name
end
```
```    
```

```rb
age = 21
if age
  puts "My age is: " + no_name
end
```
``` (NameError)
```

```rb
age = gets.chomp
if age
  puts "My age is: " + age
end
```
```My age is: 29
```

### Conditionals

Write the code for the following exercise inside of the `app.rb` located in this repo. Run/test your code using `ruby app.rb` in the Terminal.

#### Write FizzBuzz in Ruby!

Fizz-Buzz is a classic coding exercise that you can create using your knowledge of conditionals and loops. Implement code that does the following...

* Counts from 1 to 100 and prints out something for each number.
* If the number is divisible by 3, print `"Fizz"`.
* If the number is divisible by 5, print `"Buzz"`.
* If the number is divisible by both 3 and 5, print `"FizzBuzz"`.
* If the number does not meet any of the above conditions, just print the number.

Your output should look something like this...
`

(1..100).each do |n|
    i_3=(n%3==0)
    i_5=(n%5==0)
    case
        when i_3&&i_5
            puts 'fizzbuzz'
        when i_3
            puts 'fizz'
        when i_5
            puts 'buzz'
        else
            puts n
    end
end

<details>
  <summary><strong>We haven't covered loops yet, so to get you started...</strong></summary>

  ```rb
  i = 1
  while i <= 100
    # Your code goes in here.
  end
  ```

</details>
