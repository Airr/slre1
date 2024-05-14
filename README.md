SLREv1 - Original Version of the Super Light Regular Expression library

SLRE is an ANSI C library that implements a tiny subset of Perl regular expressions. It is primarily targeted for developers who want to parse configuation files, where speed is unimportant. It is in single .c file, easily modifiable for custom needs. For example, if one wants to introduce a new metacharacter, '\i', that means 'IP address', it is easy to do so.
Features

    Crossplatform - pure ANSI C
    Very simple API
    Light: about 5kB of code when compiled
    Uses no dynamic memory allocation
    Thread safe 

Supported RE Syntax

      ^               Match beginning of a buffer
      $               Match end of a buffer
      ()              Grouping and substring capturing
      [...]           Match any character from set
      [^...]          Match any character but ones from set
      \s              Match whitespace
      \S              Match non-whitespace
      \d              Match decimal digit
      \r              Match carriage return
      \n              Match newline
      +               Match one or more times (greedy)
      +?              Match one or more times (non-greedy)
      *               Match zero or more times (greedy)
      *?              Match zero or more times (non-greedy)
      ?               Match zero or once
      \xDD            Match byte with hex value 0xDD
      \meta           Match one of the meta character: ^$().[*+?\

License


  ----------------------------------------------------------------------------
 * "THE BEER-WARE LICENSE" (Revision 42):
 * Sergey Lyubka wrote this file. As long as you retain this notice you
 * can do whatever you want with this stuff. If we meet some day, and you think
 * this stuff is worth it, you can buy me a beer in return.
  ----------------------------------------------------------------------------

Author

Copyright © by Sergey Lyubka (valenok at gmail dot com), with additional code by Armando Rivera.
