## Enumerable

### Use `next` in map still return `nil`

```ruby
> [1, 2, 3].map { |n| next if n.even?; n }
=> [1, nil, 3]
```
