## Regular Expression

### Regular Literal

Do not need to escape forward slash

```ruby
%r{http://github\.com}
```

### Match UTF-8 Chinese

```
/\p{Han}+/u
```

### Match Japanese (Hiragana and Katagana)

```
/\p{Hiragana,Katakana}+/u
```

