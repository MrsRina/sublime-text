<!-- COLOR SCHEME TEST "gray-matter/Gray Matter Light.tmTheme" "Markdown" -->

## Markdown Tests

#### Font Styles

A paragraph containing **bold style A** text.
<!--                     ^^^^^^^^^^^^ fs=bold  -->

A paragraph containing __bold style B__ text.
<!--                     ^^^^^^^^^^^^ fs=bold  -->

A paragraph *italics style A* test.
<!--         ^^^^^^^^^^^^^^^ fs=italic  -->

A paragraph _italics style B_ test.
<!--         ^^^^^^^^^^^^^^^ fs=italic  -->

Sometimes these can be in**sid**e cer*ta*in words.
<!--                     ^^ fg=#B9B9B9 -->

#### Links

A paragraph containing [link text here](http://daringfireball.net).
<!--                   ^ fg=#B9B9B9     ^^^^^^^^^^^^^^^^^^^^^^^^^ fg=#B9B9B9-->

This is a [normal link with a title](http://daringfireball.net "Has a title") style.
<!--      ^ fg=#B9B9B9 ^^^^ fg=#3C3C3C ^ fg=#B9B9B9  ^^^^^^^^^^^^^^^^^^^^^^^ fg=#B9B9B9-->

This is a [reference link][reference_id] style.
<!--       ^ fg=#3C3C3C    ^ fg=#B9B9B9 -->

This is a [lazy reference link][] style.
<!--                          ^^^ fg=#B9B9B9 -->

This is an automatic link: <http://example.com/> style and one more <email@email.com>.
<!--                       ^^^^^^^ fg=#B9B9B9                       ^^^^^^^ fg=#B9B9B9-->

A paragraph with an
inline linebreak

[reference_id]: http://daringfireball.net "A reference link"
[lazy reference link]: http://daringfireball.net
<!--                ^^ fg=#B9B9B9 -->

#### Escaping

This is some \` escaped syntax and some other \* escaped syntax
<!--         ^ fg=#B9B9B9                     ^^ fg=#B9B9B9 -->

This is just a \ standard backtick
<!--           ^ fg=#3C3C3C -->

### Headings

# A H1

# This is an H1 #

This is an H1
=============
<!-- ^^^^^^^^ fg=#B9B9B9  -->

## A H2

## This is an H2 ##

This is an H2
-------------
<!-- ^^^^^^^^ fg=#B9B9B9  -->

### A H3

### A H3 with *italics* and **bold**
<!--           ^^^^^^^ fs=italic  -->

### A H3 with some flaws ###
<!--                     ^ fg=#B9B9B9  -->

### [A H3 that is a link](http://daringfireball.net)

### A H3 that contains `code` and a [link](http://daringfireball.net)

#### A H4

##### A H5
<!--  ^^^^ fs=bold  -->

###### A H6
<!-- ^ fg=#B9B9B9  -->

### Lists

- Note +, -, and * should be supported
- Testing _character_ **types** [here]()
* Testing nesting 1
    - level one A
    - level one B
<!--^ fg=#B9B9B9  -->
        1. level two A
        2. level two B
<!--    ^^ fg=#B9B9B9  -->
+ Testing nesting 2
    1. level one A
    2. level one B
<!--^^ fg=#B9B9B9  -->
        + level two A
        - level two B
<!--    ^ fg=#B9B9B9  -->
- #### Headings in lists
* Testing ``code`` inside
<!--      ^^^^^^^^ bg=#ededed  -->

        <html>of lists</html>
* Testing multiple

    paragraphs in lists
+ > Testing blockquotes

.

1. Testing _character_ **types** [here]()
2. Testing nesting 1
    - level one A
    - level one B
        1. level two A
        2. level two B
3. Testing nesting 2
    1. level one A
    2. level one B
        + level two A
        - level two B
4. #### Headings in lists
4. Testing ``code`` inside

        <html>of lists</html>
6. Testing multiple

    paragraphs in lists
1. > Testing blockquotes

### Blockqotes

> This is a blockquote.
<!--   ^^^^^^^^^^^^^^^^ fs=italic  -->

> This is a blockquote with a line break.
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

> This is a blockquote with a line break.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

> This is a blockquote with some nesting.
>> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.
>>> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");

### Rulers/Rules

* * *
<!--^ fg=#B9B9B9  -->

***

*****
<!--^ fg=#B9B9B9  -->

- - -
<!--^ fg=#B9B9B9  -->

---------------------------------------
<!--                                  ^ fg=#B9B9B9  -->

---------------
<!--          ^ fg=#B9B9B9  -->

### Code

This is a normal paragraph:

    This is a code block.
<!--^^^^^^^^^^^^^^^^^^^^^ bg=#ededed  -->

Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell

This is inline code: `some code here`.

    <script>
        document.location = 'http://example.com/?q=markdown+cheat+sheet';
    </script>

```
java
public class HelloWorld {
   public static void main(String[] args) {
       System.out.println("Hello, world!");
   }
}
```

~~~
java
public class HelloWorld {
   public static void main(String[] args) {
       System.out.println("Hello, world!");
   }
}
~~~

### Images

![Alt text](/path/to/img.jpg)
<!--  ^^^ fg=#3C3C3C    ^^^^^ fg=#B9B9B9 -->

![Alt text](/path/to/img.jpg "Optional title")
<!--      ^^^^^ fg=#B9B9B9 -->

### Embedded HTML

<h1><span class="test">Test</span></h1>
<img src="test" alt="test" />
<!-- ^^^^^^^^^^^^^^^^^^^^^^^^ fg=#B9B9B9  -->

### Literals

\\ a literal backslash
\` a literal backtick
\* a literal asterisk
\_ a literal underscore
\{ a literal curly braces
\[ a literal square brackets
\( a literal parentheses
\# a literal hash mark
\+ a literal plus sign
\- a literal minus sign (hyphen)
\. a literal dot
\! a literal exclamation mark

## End of Document
