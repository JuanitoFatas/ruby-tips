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

### Get allocation status

```
> ObjectSpace.count_objects

{
  :TOTAL=>309776,
  :FREE=>99,
  :T_OBJECT=>22663,
  :T_CLASS=>2091,
  :T_MODULE=>170,
  :T_FLOAT=>6,
  :T_STRING=>177856,
  :T_REGEXP=>1635,
  :T_ARRAY=>57583,
  :T_HASH=>26541,
  :T_STRUCT=>98,
  :T_BIGNUM=>2,
  :T_FILE=>4,
  :T_DATA=>12134,
  :T_MATCH=>820,
  :T_COMPLEX=>1,
  :T_RATIONAL=>1,
  :T_SYMBOL=>16,
  :T_NODE=>7817,
  :T_ICLASS=>239
}
```

### Iterate all objects

```
ObjectSpace.each_object
```

### Define things to do before GC destroy the object

```
ObjectSpace.define_finalizer
```
