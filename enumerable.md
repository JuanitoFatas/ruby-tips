## Enumerable

### Use `next` in `map` still return `nil`

```ruby
> [1, 2, 3].map { |n| next if n.even?; n }
=> [1, nil, 3]
```

### Create hash from Enumerable

```ruby
> input = [1, 2, 3, 4, 5];

> Hash[input.map do |n|
  [n, 2*n]
end]
=> { 1=>2, 2=>4, 3=>6, 4=>8, 5=>10 }

### Create hash from Enumerable (Better)

```ruby
> input = [1, 2, 3, 4, 5];

> input.inject({}) do |hash, n|
  hash.merge!(n => 2*n)
end
=> { 1=>2, 2=>4, 3=>6, 4=>8, 5=>10 }
```
