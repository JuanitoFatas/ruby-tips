# Bundler

## 001 "bundle update" in console

```ruby
definition = Bundler::Definition.build("Gemfile", "Gemfile.lock", true)
definition.resolve_remotely!
definition.lock("Gemfile.lock")
```
