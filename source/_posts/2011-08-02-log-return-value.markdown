---
layout: post
title: "Ruby: Log return value"
date: 2011-08-02 14:55
comments: true
categories: ruby
---

Если вам нужно вывести в лог возврщаемое из функции значение то можно
воспользоваться методом [tap()](http://apidock.com/ruby/Object/tap):

``` ruby
    def some_function
      complex_calculation.tap{ |v| Rails.logger.debug "returnd value = #{v}" }
    end
```
