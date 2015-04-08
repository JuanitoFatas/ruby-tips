## Hash

### Create Hash by array of even number of elements

```ruby
> Hash[:a, 1, :b, 2]

=> { :a => 1, :b => 2}
```

### Double Splat

### Replace merge with double splat

```ruby
> h1 = { a: 1 };
> h2 = { b: 2 };
> h3 = { d: 4 };
> h4 = { **h1, **h2, c: 3, **d }
=> { a: 1, b: 2, c: 3, d: 4 }
```
