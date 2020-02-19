# Hello World

- [Hello World](#hello-world)
  - [My First Program:](#my-first-program)
    - [Demystifying Some Code](#demystifying-some-code)
      - [`#include <stdio.h>`](#include-stdioh)
      - [`int main(void) {`](#int-mainvoid)
      - [`printf("Hello World!\n");`](#printf%22hello-worldn%22)
      - [`return 0;`](#return-0)
  - [Wrap up](#wrap-up)

## My First Program:

Let's write our first program. Pop open Visual Studio and create a new project and create a file called `main.c`. Once you open it up, type the following code in there:

```c
// this imports a bunch of pre-written code that we can use
#include <stdio.h>

// ┌─ `int`: The type of date being returned
// │  ┌─ `main`: The name of the function: we need to call it main so
// │  │  the program knows where to start
// │  │    ┌─ `(void): The stuff we're giving to the date. Right now,
// │  │    │  we're not giving it anything so we put void.
// │  │    │
int main(void) { // Opening curly brace. Can be here or on the next
                 // line but this signifies the beginning of a chunck
                 // of code
  printf("Hello World!\n"); // Give the characters "Hello World!\n"
                            // to the function `printf` so we can
                            // display stuff on the screen

  return 0; // return the number 0 so the computer knows the program
            // finished running successfully
} // Closing curly brace to end our code block
```

Or if you don't want comments:

```c
#include <stdio.h>
int main(void) {
  printf("Hello World!\n");
  return 0;
}
```

### Demystifying Some Code

Let's unpack all this:

#### `#include <stdio.h>`

This line is usally the first line in your code. This says "Hey Computer! Before you do anything else, I want you to get the pre-written code out of the file `stdio.h` (`STanDard Input/Output`) and add it to this program so I can use it."

#### `int main(void) {`

This is a **function definition**. This is where we **define** what the **function** does. A function in programming is basically a set of instructions that you're computer does that has a name so that way, whenever you use that name, your computer will do those steps. You can think of it like how a song is a series of notes with a name associated with it and whenever you play that song, you always play those notes in that order. For example, if you were to call up Clifford Smith and say "Sing 'Method Man'", he'd start listing off all the members of the Wu Tang Clan the same way he always does it because those are the lyrics.

In a function definition, you have the **return type** which is the type of information the function will spit out when it's done. We don't care right now _what_ it is, only it's type. Some examples are `void` (nothing), `int`, `char`, `double`.

After that, we have the **function name**. This can be anything but each project has to have a function called `main` because that's where it starts. `main` is like the beginning box on a flowchart.

Then, we have `(void)` which is saying that we're not giving the function anything. However, in other functions, you can give a list of inputs like `(int a, int b, char x)` but we won't worry about that just yet.

Lastly, we have the **curly brace '{'**. This can be on the same line as the definition or the next one. I like it on the same line but it's more common to see it on the next line.

**Same Line**

```c
int main(void) {
  return 0;
}
```

**next Line**

```c
int main(void)
{
  return 0;
}
```

Either way, these "wrap" around or group a block of code. So in our hello world function, we have our `printf` and `return` statements inside `{}` to signify that they are a part of that function and not some other function or any other code. These will have more importance later but for now, the big take-away is that you use `{}` to associate code with a function.

When you run this, it will print the characters `Hello World` and then a `newline` character (`\n`) which is the equivalent of hitting the `enter` key on your keyboard.

#### `printf("Hello World!\n");`

This line says "Run the function `printf` and give it the string `Hello World!\n`". Then we have the `;` to signify that that's the end of an instruction. In general (but not always) we end lines with `;` in C. The outcome of this line of code is that the function `printf` takes that string you gave it and prints it to the screen. That's it.

#### `return 0;`

This line tells the function `main` to spit back the number `0` to the computer. In this case, the computer takes the `0` as a sign that the program ended with a success. We'll talk more about **return statements** later.

## Wrap up

We just covered a lot. If you're feeling overwhelmed, that's normal. There's a lerning curve to this and it'll feel like you're drinking through a firehose up until it doesn't. So to help with that, don't worry about absorbing everything from this. Here are the key points:

1. Hello World is the first program you usually write
2. There are things called **functions** that are a named set of repeatable instructions for a computer
3. Every program in C has a `main` function so the computer knows where to start
4. Functions need to have `{}` around their code
5. Most lines end with a `;`
