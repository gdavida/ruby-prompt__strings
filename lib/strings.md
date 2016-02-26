---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

-sequence of characters STRUNG together

( https://www.youtube.com/watch?v=wKAdcFW5kp8 )

-enclosed in single quotes - literal, or double quotes - evaluation


# What are some examples of information that would be Strings as opposed to some other data type?

Like names or sentences or other words. Numbers can be as long as you are not intending to evaluate those numbers.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

name = "Ada Lovelace"
puts name[5]   => o
puts name[7]   => e
puts name[99]  => nothing returns

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

YES! It is possible. The negative position means you are starting from the end, with the last character being = position [-1], then the second from last character [-2] and so on...

name = "Ada Lovelace"
puts name[-6]   => v

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

-sub() method replaces just the first instance of a string with another.
-gsub() replaces all instances.

myString = "Sumeet Jain"
newString = myString.gsub("e", "!")
puts newString


( http://www.dotnetperls.com/sub-ruby )
