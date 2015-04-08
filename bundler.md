## Bundler

### "bundle update" in console

```ruby
definition = Bundler::Definition.build("Gemfile", "Gemfile.lock", true)
definition.resolve_remotely!
definition.lock("Gemfile.lock")
```

### Parallel bundle install works on Linux

```
bundle install jobs $(sysctl -n hw.ncpu)
```

### Global Parallel bundle install config on Linux

```
bundle config --global jobs $(nproc)
```

### Parallel bundle install works on OS X

```
bundle install jobs $(sysctl -n hw.ncpu)
```

### Global Parallel bundle install config on OS X

```
bundle config --global jobs $(sysctl -n hw.ncpu)
```
