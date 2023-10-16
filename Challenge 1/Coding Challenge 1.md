# **Fizz Buzz Enhanced**

It's your favourite programing challenge: Fizz Buzz, but harder.

Write a program that displays all digits to n while adhering to the following rules:

### **Display**
A new line after every 10 digits.
n must be displayed with 0 filling in the space.

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.**
```
  001 002 003 004 005 006 007 008 009 010
  [...]
  091 092 093 094 095 096 097 098 099 100
```
### **Fizz**
Fizz starts at 3
If n % fizz = 0, it should be replaced with 'fizz'.
However, it should only display the letters to the length of max int.

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.**
```
11 fi 13 14
```
If the length of the number is greater than 'fizz', then it repeat the letters.

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.** 
```
  000001 000002 fizzfi 000004
```
After every 10 numbers, fizz += 1

### **Buzz**

Buzz is the next prime number of Fizz
if n % buzz = 0, the number should be replaced with 'buzz'.
However, it should only display the letters to the length of max int.

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.** 
```
11 bu 13 14
```
If the length of the number is greater than 'buzz', then it repeat the letters

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.**
```
000001 000002 buzzbu 000004
```
Whenever Fizz updates, Buzz should update too.

**FizzBuzz**

When a n % fizz = 0 AND n % buzz = 0, it should display the allocated space equally:

&nbsp;&nbsp;&nbsp;&nbsp;**e.g.**
```
  13 14 fb 16
  1033 1034 fibu 1036
  12346783 12346784 fizzbuzz 12346786
```
**More Examples:**

**_Note: These are with standard FizzBuzz rules where fizz = 3, buzz = 5_**

**1 to 100:**
```
001 002 fiz 004 buz fiz 007 008 fiz buz 
011 fiz 013 014 fib 016 017 fiz 019 buz 
fiz 022 023 fiz buz 026 fiz 028 029 fib 
031 032 fiz 034 buz fiz 037 038 fiz buz 
041 fiz 043 044 fib buz 047 fiz 049 buz 
fiz 052 053 fiz buz 056 fiz 058 059 fib 
061 062 fiz 064 buz fiz 067 068 fiz buz 
071 fiz 073 074 fib 076 077 fiz 079 buz 
fiz 082 083 fiz buz 086 fiz 088 089 fib 
091 092 fiz 094 buz fiz 097 098 fiz buz
```

**1 to 1000:**
```
0001 0002 fizz 0004 buzz fizz 0007 0008 0009 buzz 
0011 fizz 0013 0014 fibu 0016 0017 fizz 0019 buzz 
fizz 0022 0023 fizz buzz 0026 fizz 0028 0029 fibu 
[...]
fizz 0982 0983 fizz buzz 0986 fizz 0988 0989 fibu 
0991 0992 fizz 0994 buzz fizz 0997 0998 fizz buzz
```

**1 to 10000000:**
```
00000001 00000002 fizzfizz 00000004 buzzbuzz fizzfizz 00000007 00000008 00000009 buzzbuzz 
00000011 fizzfizz 00000013 00000014 fizzbuzz 00000016 00000017 fizzfizz 00000019 buzzbuzz 
[...]
fizzfizz 09999982 09999983 fizzfizz buzzbuzz 09999986 fizzfizz 09999988 09999989 fizzbuzz 
09999991 09999992 fizzfizz 09999994 buzzbuzz fizzfizz 09999997 09999998 fizzfizz buzbuzzz
```
