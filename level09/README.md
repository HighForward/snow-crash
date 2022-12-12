# LEVEL 09

- We have the token encrypted and the level09 file is telling us how it was encrypted:
- By playing with the input a bit we figure out that its a form of an ascii array encryption, 

```
level09@SnowCrash:~$ ./level09 aaaaaaaaaaaaaaaa
abcdefghijklmnop
```

- For each char, the output is the char value + the offset of the array position written in ascii
- To decrypt the token we have to reverse the token in the way level09 program do it
- dump chars in hex to get there ASCII hex values, minus there position in the string, and reverse to ascii
