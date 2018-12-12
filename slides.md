# The Stacktrace

## Maria Mckinley



## Let's make a fancy cake
![alt text](assets/mocha-dacquoise.jpg "Mocha Dacquoise Cake")
#### Mocha Dacquoise




## Basic cake instructions:
* make meringue
* make buttercream
* make chantilly
* assemble




## Each step consists of more steps

### for example, 'make buttercream' consists of: <!-- .element: class="fragment" data-fragment-index="1" -->
* make syrup <!-- .element: class="fragment" data-fragment-index="2" -->
* whisk egg yolks <!-- .element: class="fragment" data-fragment-index="2" -->
* whisk syrup into egg yolks <!-- .element: class="fragment" data-fragment-index="2" -->




### and of course, 'make syrup' also has a couple of steps:
* In a high-sided saucepan over medium heat, add the coffee and sugar.
* Set a candy or deep-fat thermometer into the pan and heat until the mixture registers 265&deg;F.




## Code is instructions for a computer
## like a recipe is instructions for a cook




![alt text](assets/how-to-make-golden-syrup.jpg "https://nishamadhulika.com/en/788-homemade-golden-syrup.html")

[comment]: # Let's say we are currently adding the sugar to make the syrup for the buttercream for the cake.




## Things we have started, but not yet completed:

* started making cake
* started making buttercream
* started making syrup
* started adding sugar

## This is called the Stack<!-- .element: class="fragment" data-fragment-index="1" -->

#### 'make meringue' isn't there: we finished making it.<!-- .element: class="fragment" data-fragment-index="2" -->
#### 'make chantilly' isn't there: we haven't started making it.<!-- .element: class="fragment" data-fragment-index="3" -->




### What happens if something goes wrong while making the syrup?

![alt text](assets/salt_sugar.jpg "Salt or Sugar")




## The stack now shows us what we were doing when things became obvious something went wrong

```
Traceback (most recent call last):
  File "make_cake.py", line 15, in <module>
    cake = make_cake()
  File "make_cake.py", line 3, in make_cake
    buttercream=make_buttercream(buttercream_ingredients)
  File "make_cake.py", line 9, in make_buttercream
    syrup=make_syrup(coffee, salt)
  File "make_cake.py", line 13, in make_syrup
    add_sugar(salt)
TypeError: salt is not sugar
```

## This is called the stacktrace <!-- .element: class="fragment" data-fragment-index="1" -->




* make_cake()
* make_buttercream(buttercream_ingr)
* make_syrup(coffee, salt)
* add_sugar(salt)

## Read from the bottom up




## This can make for more difficult troubleshooting with code, and sometimes cakes.




![alt text](assets/cakewreck.jpg "Awesome Cake")



# Why do I care?

## Obviously useful to know what a stack trace is when someone asks for one or you want to be helpful.<!-- .element: class="fragment" data-fragment-index="0" -->

## When things go wrong, trouble shoot systematically. Step backwards, retrace your steps.<!-- .element: class="fragment" data-fragment-index="1" -->




# Review

## The stack is a list of the steps we have started, but not completed so far.<!-- .element: class="fragment" data-fragment-index="0" -->

## A stacktrace is the stack at the moment something has obviously gone wrong.<!-- .element: class="fragment" data-fragment-index="1" -->
