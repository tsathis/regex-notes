# Basic rules

## 1. `a`

Set with only a single letter string { `a` }.


## 2. ε

Set with only a empty string { "`﻿`" }

## 3. _s_|_t_

An element of sets _s_ or _t_. 
> (alternation)

e.g.: 

_s_  = { `a` } \
_t_  = { `c` }

_s_|_t_ = { `a`,`c` }

## 4. _st_ 

An element of set _s_ is cotenated with a string an element from _t_.
> (concatenation)

e.g.: 

_s_  = { `a`,`b` } \
_t_  = { `c`,`d` }

_st_ = { `ac`,`ad`,`bc`,`bd` }

## 5. _s_\*

Concatenation of any number of elements from subsets of _s_.

e.g.: 

_s_  = { `a`,`b` } 

_s_* = {  ε,`a`,`b`,`aa`,`ab`,`ba`,`bb`,`aaa`, ... }



# Properties

## Precedence

1. **\***
2. **concatenation**
3. **\|**

e.g.:

`a|ab*` = `a|(a(b*))`

## Algebraic properties

- (_r_|_s_|)_t_ = _r_|_s_|_t_ = _r_|(_s_|_t_) 
- _s_|_t_ = _t_|_s_
- _s_|_s_ = _s_
- _s_ ε = _s_ =  ε _s_
- (_rs_)|_t_ = _rst_ = _r_(_st_)
- _r_ ( _s_ | _t_ ) = _rs_ | _rt_
- ( _r_ | _s_ ) _t_  = _rt_ | _st_
- (_s_\*)\* = _s_\*
- _s_\*_s_\* = _s_\*

## Shorthands

- _s_? = _s_\|ε
- _s_+ = _ss_* = _s_*_s_
- [_st_] = _s_|_t_ 
