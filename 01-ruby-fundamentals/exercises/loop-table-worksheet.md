# Loop Table Worksheet!


1) Complete the following loop table by filling in the values for **loop count**, **value of x**, and **output**.

```ruby
[2,5,8,11,14].each do |x|
  puts 2 * x + 7
end
```

| loop count | value of x  | new value:  |
|:---:|:---:|:---:|
| 0 | 2  | 11 |
| 1 | 5  | 17 |
| 2 | 8  | 23 |
| 3 | 11 | 29 |
| 4 | 14 | 35 |


2) Complete the following loop table by filling in the values for **loop count**, **value of critter**, and **output**.
```ruby
["kittens", "meerkats", "red pandas"].each do |critter|
  affirmation = "I am as amazing as " + critter + "!"
  puts affirmation
end
```
| loop count | value of critter | affirmation | output |
|:---:|:---:|:---|:---| 
| 0 | "kittens" | "I am as amazing as" | "I am as amazing as kittens!" |
| 1 | "meerkats" |  "I am as amazing as" | "I am as amazing as meerkats!" |
| 2 | "red pandas" |  "I am as amazing as" | "I am as amazing as red pandas!" |


3) Complete the following loop table by filling in the values for **loop count**, **value of letter**, **value of s1**, **value of s2**, and **output**.
```ruby
a = ["m", "p", "e", "u", "o", "r", "w", "r"]
s1 = ""
s2 = ""

a.each do |letter|
  if (a.index(letter))%2==0
    s1=s1+letter
    puts s1
  else
    s2=s2+letter
    puts s2
  end
end
```
| loop count | value of letter | value of s1 | value of s2 | output |
|:---:|:---:|:---:|:---:|:---:|
| 0 | "m" | "m" | "" | "m" |
| 1 | "p" | "m" | "p" | "p" |
| 2 | "e" | "me" | "p" | "me" |
| 3 | "u" | "me" | "pu" | "pu" |
| 4 | "o" | "meo" | "pu" | "meo" |
| 5 | "r" | "meo" | "pur" | "pur" |
| 6 | "w" | "meow" | "pur" | "meow" |
| 7 | "r" | "meow" | "purr" | "purr" |
