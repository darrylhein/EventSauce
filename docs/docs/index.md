---
permalink: /docs/
title: Event sourcing for PHP
hide_title: true
published_at: 2018-02-21
updated_at: 2019-06-12
---

<div class="text-center mb-8 max-w-md">
    <img id="logo" src="/static/logo.svg" height="150px" width="150px" alt="EventSauce">
    <h1 class="text-grey-darkest mt-1">
        Event<span class="text-red">Sauce</span>
    </h1>
</div>

[![Source Code](https://img.shields.io/badge/source-eventsaucephp/eventsauce-blue.svg?style=flat-square)](https://github.com/eventsaucephp/eventsauce)
[![Code Quality](https://img.shields.io/scrutinizer/g/EventSaucePHP/EventSauce.svg?style=flat-square)](https://scrutinizer-ci.com/g/EventSaucePHP/EventSauce/?branch=master)
[![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/EventSaucePHP/EventSauce.svg?style=flat-square)](https://scrutinizer-ci.com/g/EventSaucePHP/EventSauce/?branch=master)
[![Travis](https://img.shields.io/travis/EventSaucePHP/EventSauce.svg?style=flat-square)](https://travis-ci.org/EventSaucePHP/EventSauce)
[![Packagist Version](https://img.shields.io/packagist/v/eventsauce/eventsauce.svg?style=flat-square)](https://packagist.org/packages/eventsauce/eventsauce)
[![Packagist](https://img.shields.io/badge/packagist-eventsauce/eventsauce-orange.svg?style=flat-square)](https://packagist.org/packages/eventsauce/eventsauce)
![php >=7.2](https://img.shields.io/packagist/php-v/eventsauce/eventsauce.svg?style=flat-square)


# What is EventSauce?

EventSauce is a no-nonsense event sourcing library for PHP with a focus on developer
experience and productivity. This library was developed with the idea that you should
be able to add event sourced parts to your application with ease. No application-wide
rewrites and no big investments upfront. The core is built around a set of (tiny)
interfaces, which gives you the freedom to choose the tools that meet your requirements.

Many parts of the library are extremely pragmatic in nature. You're encouraged to take
control over it. It allows everything from  custom storage adapter to highly customizable
message dispatching setups.

EventSauce puts the focus on event sourcing, not on things that happen around event
sourcing. It does not require you to follow CQRS patterns. It does not require you
to use a command-, event-, or query-bus. By doing so, it allows developers to use
event sourcing for parts of their application more easily.

## Why _not_ use EventSauce?

The library is focused purely around event sourcing, **not** full-blown CQRS/ES. If
you need that, I recommend checking out [Prooph](https://github.com/prooph) or
[Broadway](https://github.com/broadway/broadway). These libraries have a higher level
of entry but provide an "everything you need is right here" experience.

## Disclaimer

Solving problems using event sourcing requires a very different mindset when compared
to traditional PHP-OOP software modeling. It's less focused about state and more
about processes, transitions, and communication in general. Event sourcing is also not
simple. It's built on a body of knowledge that is inherently complex. There are many
concepts that come into play that build off one another.

However, event sourcing also provides an easier way to model a variety of issues. It's
a remedy against storing "work in progress" entities. It's a better fit when modeling
anything where the transition is just as important as the end result.
