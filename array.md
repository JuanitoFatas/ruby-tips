## Array

### Array literal of String

```
> %w(i have a dream)
=> ["i", "have", "a", "dream"]
```

### Array literal of Symbol

```
> %i(i have a dream)
=> [:i, :have, :a, :dream]
```

### Create consecutive elements from splat and Range.

```ruby
> [*1..10]
=> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

> [*:a..:z]
=> [:a, :b, :c, :d, :e, :f, :g, :h, :i, :j, :k, :l, :m, :n, :o, :p, :q, :r, :s, :t, :u, :v, :w, :x, :y, :z]
```
