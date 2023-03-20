---
title: Using Java
layout: default
nav_order: 2
parent: Getting Started
---

# Getting Started with Java
We've prepared a Java template with a simple input/output interface for any Java users. 

**Note: the input for the Java template is slightly different from that on the [guide](https://docs.battlesnake.com/api) since we've made the interface more Java-friendly. Keep reading for details.**


# Hosting your server

[Start your Battlesnake on Repl.it](https://replit.com/@JimmyLiu3/starter-snake-java?v=1){: .btn .btn-blue }

Click the link above and press **"Fork"** on the top right corner to get your snake started.

If you wish to test and host your server through other means, click [**here**](https://github.com/ji-mmyliu/starter-snake-java) to access the template from Github.

## Building your Battlesnake
Head to `Main.java` to start building your snake! This is the only file that you need to write to.

### Reading Input
You will need to read the input from `input.txt` using Java's `FileReader`. A sample code stub should be viewable in `Main.java`.

First, you will read an $$ 11 \times 11 $$ grid of characters, describing the Battlesnake board.

* `H` represents your snake's head
* `B` represents a segment of your snake's body
* `T` represents your snake's tail

* `h` represents an enemy snake's head
* `b` represents a segment of an enemy snake's body
* `t` represents a an enemy snake's tail

* `.` represents an empty space
* `f` represents a food pellet

#### Sample Input (arrives from `input.txt`)
```
.....BBH...
.....B.....
..TBBB.....
...........
...........
..t..f.....
..b........
..b........
..b........
..h........
......f....
87
```
The above sample board contains your snake at the top, an enemy snake on the bottom left, and two food pellets: one in the middle and one on the bottom. The `87` indicates that your snake still has 87 of 100 hunger points remaining (eating a food pellet refills your snake to 100 hunger points).

## Writing Output
After calculating the move that you want your Battlesnake to make, output it using `System.out.println()`. The list of possible moves are:
1. `up`
2. `down`
3. `left`
4. `right`

<script type="text/javascript" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML"></script>
