# Artusi
Let’s use commands we just learned to manipulate the files and directories of Artusi, an arts supply Store.

## Tasks

* 1.
Print the working directory.
```pwd```

* 2.
List all contents in the current directory, including hidden files and directories.

```ls -a```

* 3.
List all contents, in long format.

```ls -l```

* 4.
List all contents, including hidden files and directories, in long format, ordered by the date and time they were last modified.

```ls -alt```

* 5.
Change directories to the pencils/ directory. The relative path of the pencils directory is drawing/pencils/.

```/home/ccuser/workspace/artusi```
and from our ls command, we know drawing/ is a directory inside the current directory. Since we’re told pencils/ is inside drawing/, we simply need to change directory like 
so:

```cd drawing/pencils```

* 6.
List all contents in the current working directly, including hidden files and directories.

```ls -a```

* 7.
Copy the file color.txt to graphite.txt.

```cp color.txt graphite.txt```

You can use the following commands to confirm the result of the above cp statement:

```cat color.txt```

and

```cat graphite.txt```
(cat is a command that outputs the contents of a file)

* 8.
Change directories into the charcoal/ directory. The relative path to the charcoal directory is ../charcoal/.

```/home/ccuser/workspace/artusi/drawing/pencils/charcoal/``` is another directory inside the directory drawing/. That means we need to go up a directory level to drawing/ 
using .., and from there go into charcoals/. So our cd 
statement would be:

```cd ../charcoals```

* 9.
Copy the file compressed.txt to vine.txt.

```cp compressed.txt vine.txt```

You can use the following commands to confirm the result of the above cp statement:

```cat compressed.txt```

and

```cat vine.txt```

* 10.
Copy the file vine.txt to pencils/color.txt. The relative path of the latter is ../pencils/color.txt.

```cp vine.txt ../pencils/color.txt```

You can use the following commands to confirm the result of the above cp statement:

```cat vine.txt```

and

```cat ../pencils/color.txt```

* 11.
From the charcoal/ directory, change directories to the painting/ directory. The relative path is ../../painting/.


The current directory is

```/home/ccuser/workspace/artusi/drawing/charcoal/painting/``` is another directory inside the directory artusi/. That means we need to go up two directory levels to artusi/ 
using ../.., and from there go into painting/. So our
cd statement would be:

```cd ../../painting```

* 12.
Print the working directory.

```pwd```

* 13.
List all contents, in long format, including the hidden files and directories, ordered by the date and time they were last modified.

```ls -alt```

* 14.
Change directories to the brushes/ directory.

```/home/ccuser/workspace/artusi/painting```

and from our ls command from the last step, we know brushes/ is a directory inside the current directory. So our cd command would simply be this:

```cd brushes```

* 15.
List all contents, in long format, including the hidden files and directories, ordered by the date and time they were last modified.

```ls -alt```

* 16.
Copy the files starting with the letter f from the brushes/ directory to the paint/ directory. The path to the paint/ directory is ../paint/.

Without changing directories, list the files and directories of the paint/ directory.

The source file(s) are all .txt files starting with f, which we can shorthand as f*.txt (* is wildcard).
The destination is ../paint/
Putting it all together, the cp command would be:

```cp f*.txt ../paint/```
To look at the ../paint/ directory, use ls.

```ls ../paint/```
What you see should confirm that your cp command worked!

* 17.
Change directories to the sculpting/ directory. The relative path is ../../sculpting/

```/home/ccuser/workspace/artusi/painting/brushes/sculpting/``` is another directory inside the directory artusi/. That means we need to go up two directory levels to artusi/ 
using ../.., and from there go into sculpting/. So our
cd statement would be:

```cd ../../sculpting. ```

* 18.
List all contents, in long format, including the hidden files and directories, ordered by the date and time they were last modified.

```ls -alt```

* 19.
Change directories into the clay/polymer/ directory, and list all contents of the directory.

```/home/ccuser/workspace/artusi/sculpting/clay/``` is a directory inside the current one so we can change directories like so:

```cd clay/polymer```

Now view the contents in the current directory:

```ls```

* 20.
Move airdry.txt into the ceramic/ directory. The relative path to the is ../ceramic/.

```mv airdry.txt ../ceramic/```
You can use the following commands to confirm the result of the above move:

```ls```
to make sure airdry.txt is no longer in the current directory and

```ls ../ceramic/```
to see airdry.txt in the destination directory.

* 21.
Change directories into the ceramic/ directory.

```cd ../ceramic```
You can confirm you changed into the correct directory using

```pwd```

* 22.
List all contents, including hidden files and directories.

```ls -a```

* 23.
Remove earthenware.txt from the current directory.

```rm earthenware.txt```

You can confirm the removal of the file using

```ls```

to see the updated contents of the directory.

* 24.
Change directories one level up back to the clay/ directory.

```cd ..```
You can confirm you changed into the correct directory using

```pwd```

* 25.
Take a look at the contents of the current directory clay/. Delete the dough/ directory.

Since dough/ is a directory, our command would look like this:

```rm -rf dough```

* 26.
Change directories two levels up back to the artusi/ directory. Print the working directory.

```cd ../..```
Let’s confirm the current directory using

pwd
