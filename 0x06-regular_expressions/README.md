# 0x06. Regular expression
This looks at regex: modifiers, brackets, meta characters.

## Concept
1. [Regular-Expressions.info](https://www.regular-expressions.info/)
2. [JavaScript RegExp Reference](https://www.w3schools.com/jsref/jsref_obj_regexp.asp)
3. [Rubular](https://rubular.com/)
4. [Regular Expression 101](https://regex101.com/)

## Resources
1. [Regular expressions - basics](https://www.slideshare.net/slideshow/introducing-regular-expressions/63676155)
2. [Regular expressions - advanced](https://www.slideshare.net/slideshow/advanced-regular-expressions-80296518/80296518)
3. [Regular Expressions: Now You Have Two Problems](https://blog.codinghorror.com/regular-expressions-now-you-have-two-problems/)
4. [Rubular is your best friend](https://rubular.com/)
5. [Learn Regular Expressions with simple, interactive exercises](https://regexone.com/)

## Background Context
For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties. Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the //:
```
sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a
```
- The first line of all your Bash scripts should be exactly #!/usr/bin/env ruby
- All your regex must be built for the Oniguruma library

## Summary
A regular expression, commonly called a “regexp”, is a sequence of characters that define a search pattern.  It is mainly for use in pattern matching with strings, or string matching (i.e. it operates like a “find and replace” command).

**JavaScript RegExp Reference**
- Modifiers: g, i, m, d.
- Brackets: [abc], [^abc], [0-9], [^0-9], (x|y)
- Metacharacters: ., \d, \s, \w, \b, \D, \S, \W, \B, \0, \n, \f, \r, \t, \v, \xxx, \xdd, \uddd.
- Quantifiers: n+, n*, n?, n{X}, n{X, Y}, n{X,}, n$, ^n, ?=n, ?!n.
- Object properties: constructor, global, ignoreCase, lastIndex, multiline, source.
- Object methods: exec(), test(), toString().

**Rubular regex quick reference**

![summary0](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/9b17d949-23dd-4bd0-860f-f9d3806a6c41)

****
- Repitition token: {m, n}, ?, +, -
  1. Greedy(backtracks): *, +, ?, {m, n}
  2. Lazy(backtracks): *?, +?, ??, {m, n}?
  3. Possesive(does not backtrack): *+, ++, ?+, {m, n}+
- Anchor token: ^, $, \A, \Z
- Character token: [a-zA-Z0-9], [^a-zA-Z0-9], [a-zA-Z0-9]+, [1st -[2nd]].
- Shortcut token: \d, \s, \w, \D, \S, \W
- The dot(.)

## Tasks

