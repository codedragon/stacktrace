# The Stacktrace

## Maria Mckinley



## Let's make a fancy cake
![alt text](assets/mocha-dacquoise.jpg "Mocha Dacquoise Cake")




## Basic cake instructions:
* make meringue
* make buttercream
* make chantilly
* assemble




## Each step consists of more steps

### for example make buttercream consists of: <!-- .element: class="fragment" data-fragment-index="1" -->
* make syrup
* whisk egg yolks
* whisk syrup into egg yolks




### and of course make syrup has a couple of steps:
* In a high-sided saucepan over medium heat, add the coffee and sugar. 
* Set a candy or deep-fat thermometer into the pan and heat until the mixture registers 265&deg;F.




## Code is instructions for a computer
## like a recipe is instructions for a cook




## Let's say we are currently making the syrup for our cake




## A stack is a list of the steps we have started, but not completed so far:

* make cake
* make buttercream
* make syrup

#### make meringue is not there, because we finished making the meringue.
#### make chantilly isn't there, because we have not started making the chantilly.




## What happens if something goes wrong while making the syrup? 
## We end up with a stack as shown above:

```
Traceback (most recent call last):
  File "make_cake.py", line 15, in <module>
    make_cake(ingredients)
  File "make_cake.py", line 3, in make_cake
    buttercream=make_buttercream(syrup, egg_yolks)
  File "make_cake.py", line 9, in make_buttercream
    syrup=make_syrup(coffee, sugar) 
  File "make_cake.py", line 13, in make_syrup
    add_sugar(salt)
TypeError: salt is not sugar
```




## The stack is a list of the steps we have started, but not completed so far

## A stacktrace is the stack at the moment something has obviously gone wrong

