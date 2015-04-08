## Control Flow

### Early return

```ruby
def process_odd_number(number)
  return if number.even?

  process(number)
end
```
