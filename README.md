# What are Regular Expressions?
Regular expressions are a way to describe patterns in a string data. They form a small language of its own, which is a part of many programming languages like Javascript, Perl, Python, Php, and Java.

Regular expressions allow you to check a string of characters like an e-mail address or password for patterns, to see so if they match the pattern defined by that regular expression and produce actionable information.

## Creating a Regular Expression
There are two ways to create a regular expression in Javascript. It can be either created with RegExp constructor, or by using forward slashes ( / ) to enclose the pattern.

Regular Expression Constructor:

Syntax: new RegExp(pattern[, flags])

Example:

var regexConst = new RegExp('abc');

Regular Expression Literal:
Syntax: /pattern/flags

Example:

var regexLiteral = /abc/;

There might also be cases where you want to create regular expressions dynamically, in which case regex literal won’t work, so you have to use a regular expression constructor.

No matter which method you choose, the result is going to be a regex object. Both regex objects will have same methods and properties attached to them.

Since forward slashes are used to enclose patterns in the above example, you have to escape the forward slash ( / ) with a backslash ( \ ) if you want to use it as a part of the regex.

### Regular Expressions Methods
There are mainly two methods for testing regular expressions.

#### RegExp.prototype.test()
This method is used to test whether a match has been found or not. It accepts a string which we have to test against regular expression and returns true or false depending upon if the match is found or not.

For example:

var regex = /hello/;
var str = 'hello world';
var result = regex.test(str);
console.log(result);
// returns true
RegExp.prototype.exec()
This method returns an array containing all the matched groups. It accepts a string that we have to test against a regular expression.

For example:

var regex = /hello/;
var str = 'hello world';
var result = regex.exec(str);
console.log(result);
// returns [ 'hello', index: 0, input: 'hello world', groups: undefined ]
// 'hello' -> is the matched pattern.
// index: -> Is where the regular expression starts.
// input: -> Is the actual string passed.
