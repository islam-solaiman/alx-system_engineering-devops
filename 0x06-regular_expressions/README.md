# 0x06. Regular expression

# Background Context

For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the //:

sylvain@ubuntu$ cat example.rb<br>
/#!/usr/bin/env ruby<br>
puts ARGV[0].scan(/127.0.0.[0-9]/).join<br>
sylvain@ubuntu$<br>
sylvain@ubuntu$ ./example.rb 127.0.0.2<br>
127.0.0.2<br>
sylvain@ubuntu$ ./example.rb 127.0.0.1<br>
127.0.0.1<br>
sylvain@ubuntu$ ./example.rb 127.0.0.a<br>

# Resources

### Read or watch:

[Regular expressions - basics](https://www.slideshare.net/neha_jain/introducing-regular-expressions)<br>
[Regular expressions - advanced](https://www.slideshare.net/neha_jain/advanced-regular-expressions-80296518)<br>
[Rubular is your best friend](https://rubular.com/)<br>
[Use a regular expression against a problem: now you have 2 problems](https://blog.codinghorror.com/regular-expressions-now-you-have-two-problems/)<br>
[Learn Regular Expressions with simple, interactive exercises](https://regexone.com/)<br>

# Requirements

## General

	- Allowed editors: vi, vim, emacs
	- All your files will be interpreted on Ubuntu 20.04 LTS
	- All your files should end with a new line
	- A README.md file, at the root of the folder of the project, is mandatory
	- All your Bash script files must be executable
	- The first line of all your Bash scripts should be exactly #!/usr/bin/env ruby
	- All your regex must be built for the Oniguruma library

# Regular expression

In this project, I learned how to use regular expressions. All my regex is built for the Oniguruma library.

## Tasks :page_with_curl:

_Note: Each Ruby script in the project matches regular expressions based on an argument passed to it via the command line._

* **0. Simply matching Holberton**
  * [0-simply_match_holberton.rb](./0-simply_match_holberton.rb): Ruby script that matches the regular expression `School`.

* **1. Repetition Token #0**
  * [1-repetition_token_0.rb](./1-repetition_token_0.rb): Ruby script that matches the regular expression `hbn` with between 2-5 `t`'s in between `hb` and `n`.

* **2. Repetition Token #1**
  * [2-repetition_token_1.rb](./2-repetition_token_1.rb): Ruby script that matches the regular expression `hn` with 0 or 1 occurrences of `b` and 0 or 1
  occurrences of `t` in between `h` and `n`.

* **3. Repetition Token #2**
  * [3-repetition_token_2.rb](./3-repetition_token_2.rb): Ruby script that matches the regular expression `hbn` with 1 or more `t`'s in between `hb` and `n`.

* **4. Repetition Token #3**
  * [4-repetition_token_3.rb](./4-repetition_token_3.rb): Ruby script that matches the regular expression `hbn` with 0 or more `t`'s in between `hb` and `n`.

* **5. Not quite HBTN yet**
  * [5-beginning_and_end.rb](./5-beginning_and_end.rb): Ruby script that matches a regular expression starting with `h` and ending with `n` with any single character in between.

* **6. Call me maybe**
  * [6-phone_number.rb](./6-phone_number.rb): Ruby script that matches a regular expression representing a 10-digit phone number.

* **7. OMG WHY ARE YOU SHOUTING?**
  * [7-OMG_WHY_ARE_YOU_SHOUTING.rb](./7-OMG_WHY_ARE_YOU_SHOUTING.rb): Ruby script that matches regular expressions of uppercase letters.

* **8. Textme**
  * [100-textme.rb](./100-textme.rb): Ruby script that runs statistics on TextMe app text message transcations.
  * Output: `[SENDER],[RECEIVER],[FLAGS]` where
    * `[SENDER]` is the sender phone number or name (including country code if present).
    * `[RECEIVER]` is the receiver phone number or name (including country code if present).
    * `[FLAGS]` is the flags that were used.

