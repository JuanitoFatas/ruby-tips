## Regular Expression

### Regular Literal

Do not need to escape forward slash

```ruby
%r{http://github\.com}
```

### Character Properties

http://ruby-doc.org/core-2.2.1/Regexp.html#class-Regexp-label-Character+Properties

### Match UTF-8 Chinese

```
/\p{Han}+/u
```

### Match Japanese (Hiragana and Katagana)

```
/\p{Hiragana,Katakana}+/u
```

