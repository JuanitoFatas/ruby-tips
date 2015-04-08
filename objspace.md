## [ObjectSpace](http://ruby-doc.org/stdlib-2.2.1/libdoc/objspace/rdoc/ObjectSpace.html)

### How to require

```
require "objspace"
```

### Measure a object's memory size

```
ObjectSpace.memsize_of BasicObject
=> 148042
```

### Memory size of all alive objects

```
ObjectSpace.memsize_of_all
```
