<style>
.reveal section img { background:none; border:none; box-shadow:none; }
</style>

hi

---

this is our talk

---

its about software

---

but really its about life

---

![test](./static/life.jpg)

---

the life of living with software

---

![](static/frustration.jpg)

---

first

---

im dan

---

im matt

---

we work in software

---

![dd](./static/date-a-dog.jpg)

---

![](./static/dog-1.jpg)

---

![](./static/dog-2.jpg)

---

![](./static/datadog.png)

---

we are a happy place

---

![](./static/sad1.jpg)

---

people love working here

---

![](./static/sad3.jpg)

---

they are very happy

---

![](./static/sad2.jpg)

---

and content with their jobs

---

![](./static/sad4.jpg)

---

our customers love us

---

![](static/twitter-hate2.png)

---

we are very stable

---

![](static/twitter-down.png)

---

our apis are clean and widely loved

---

![](static/twitter-hate1.png)

---


being a software engineer is great too

---

![](static/manager.jpg)

---

the workplace is very safe

---

![](static/rsi.jpg)

---

you get to be on the computer all day

---

![](static/computer-people-1.png)

---

![](static/computer-people-2.png)

---

which is what you would be doing anyway

---

![](static/computer-people-3.png)

---

![](static/computer-people-4.png)

---

some engineers work in open offices

---

![](static/open-office.png)

---

some work in closed offices

---

![](static/closed-office.png)

---

you get to work with huge nerds

---

![](static/rms.png)

---

_no one showers_

---

![](static/no-shower.jpg)

---

managers are dumb

---

![](static/dumb-manager.png)

---

computers are hard

---

![](static/confused-grandma.png)

---

no one talks to you

---

this one might be a perk

---

yeah, strike that one off dan

---

<strike>
no one talks to you
</strike>

---

thanks matt

---

# *KANBAN*

---

![](static/fried-kanban.png)

---

lots of talk about agility

---

and sprints

---

but cardio is hard

---

![](static/tired-engineer.png)

---

people think you fix printers

---

![](static/printer-1.jpg)

---

people ask you to fix printers

---

![](static/printer-2.jpg)

---

you end up fixing printers

---

![](static/printer-3.png)

---

deadlines are unreasonable

---


code reviews can be traumatic


---

![](static/manny-pr-comments.png)

---

![](static/pr-sucks.gif)

---

waterfall doesnt work

---


![](static/tlc.gif)


---

insert agile joke here

---

# PAUSE FOR CHANGEOVER

---

ok, so software engineering sucks

---

but software is good, right?

---

we write a lot of python & go at Datadog

---

lets talk about python

---

```python
>>> True == False
False
```

---

```python
>>> 2 ** 8
256
```

---

```python
>>> True ** False == True
```

---

```python
True
```

---

wat

---

![](static/wat-1.png)

---

```python
>>> 1 ** 0 == 1
```

---

lets talk about python

---

```python
>>> type(1) == type(-1)
True
```

---


```python
>>> 1 ** 1 == 1 ** -1
True
```

---


```python
>>> type(1 ** 1) == type(1 ** -1)
```

---

```python
False
```

---

wat

---

![](static/wat-2.png)

---

```python
>>> type(1 ** -1) == float
True
```

---

lets talk about python

---


```python
>>> a = ([],)
>>> a[0].extend([1])
>>> a[0]
[1]
```

---

```python
>>> a[0] += [2]
```

---

```python
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  TypeError: 'tuple' object does not support item assignment
```

---

```python
>>> a[0]
```

---

```python
[1, 2]
```

---

wat!?!?!

---

![](static/wat-3.png)

---

lets talk about go

---


```go
package main

import (
    "math"
    "fmt"
)

func main() {
    a := math.MaxUint64
    fmt.Println(a)
}
```

---


```go
# command-line-arguments
./main.go:9:4: constant 18446744073709551615 overflows int
```
---

wat

---

![](static/wat-4.png)

---

lets talk about go

---

```go
func err1() error {
    var err error
    fmt.Println(err == nil)
    return err
}

func main() {
    err := err1()
    fmt.Println(err == nil)
}
```

---

```go
true
true
```

---

no wat this makes sense

---

![](static/think.jpg)

---

```go
type MyError string

func(me MyError) Error() string {
    return string(me)
}

func err2() error {
    var err *MyError
    fmt.Println(err == nil)
    return err
}

func main() {
    err := err2()
    fmt.Println(err == nil)
}
```

---


```go
true
false
```
---

`nil` is a tricky beast

---

Null References: The Billion Dollar Mistake

---


```go
package main

import "fmt"

func main() {
    true := false
    fmt.Println(true)
}
```

---


```go
false
```

---

wat

---

![](static/wat-5.png)

---

so software is complicated

---

and convoluted

---


it ages quickly

---

and constantly reinvents itself

---

# PAUSE FOR SECOND CHANGEOVER

---

what did we learn

---

all software is terrible

---

at datadog we help make software reliable

---


with state of the art monitoring and observability tools

---

you can run software with piece of mind

---

![](static/datadog.gif)

---

![](static/datadog2.gif)

---

![](static/datadog3.gif)

---

If you want more info

---

jc@datadoghq.com

---
