# Akkeris Metrics

> A tale of tracking down performance issues.

+++

### Akkeris Alerts

```
aka alerts:memory
aka alerts:5xxx
```

+++

### Grafana

![Memory](images/memory.png)
![Requests](images/requests.png)

+++

![Graph](images/graph-all-the-things.jpg)

+++

### l2met

Turn these:
```ruby
$stdout.puts("measure#db.latency=4ms")
$stdout.puts("count#db.vaccum=1")
$stdout.puts("sample#db.size=100GB")
```

Into this:

![img](http://f.cl.ly/items/2R0h1x1b3V0Y0z0l1t1n/Screen%20Shot%202013-07-30%20at%209.59.52%20PM.png)

+++

### Akkeris Metric Tagging

```ruby
$stdout.puts("measure#request.duration=4ms tag#controller=UsersController")
$stdout.puts("measure#request.duration=15ms tag#controller=UsersController")
$stdout.puts("measure#request.duration=64ms tag#controller=Companies")
```

+++

### Rails Instrumentation

![Rails](images/rails_instrumentation.png)
