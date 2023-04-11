# Work on project

**Description**

Now let's consider a case when you need a lot of coffee. Maybe you're hosting a party with a lot of guests! In these circumstances, it's better to make preparations in advance.

So, we will ask a user to enter the desired amount of coffee, in cups. Given this, you can adjust the program by calculating how much water, coffee, and milk are necessary to make the specified amount of coffee.

Of course, all this coffee is not needed _right_ now, so at this stage, the coffee machine doesn't actually make any coffee yet.

**Objectives**

Let's break the task into several steps:

1. First, read the numbers of coffee drinks from the input.
2. Figure out how much of each ingredient the machine will need. Note that one cup of coffee made on this coffee machine contains _200 ml_ of water, _50 ml_ of milk, and _15 g_ of coffee beans.
3. Output the required ingredient amounts back to the user.

**Examples**

The greater-than symbol followed by a space (`>` ) represents the user input. Note that it's not part of the input.

**Example 1:** _a dialogue with a user might look like this_

```
Write how many cups of coffee you will need:
> 25
For 25 cups of coffee you will need:
5000 ml of water
1250 ml of milk
375 g of coffee beans
```

**Example 2:** _here is another dialogue_

```
Write how many cups of coffee you will need:
> 125
For 125 cups of coffee you will need:
25000 ml of water
6250 ml of milk
1875 g of coffee beans
```

My code:

```kotlin
package machine

fun main() {
    println("Write how many cups of coffee you will need:")
    print("> ")
    val coffee: Int = readln().toInt()
    println("For 25 cups of coffee you will need:")
    println("${200 * coffee} ml of water")
    println("${50 * coffee} ml of milk")
    println("${15 * coffee} g of coffee beans")
}
```
