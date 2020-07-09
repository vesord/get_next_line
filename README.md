# get_next_line

## Description
Calling function `get_next_line()` in a loop will then allow to read the text available on a file descriptor one line at a time until the EOF.

It was made due to my studying in 21-school, Russia. 

The main goal of project is learn how to use static variables in C.

## Usage

Just add all files to your project.

## Info

<table>
  <tr>
    <td> <b>Prototype</b> </td> <td> <code>int get_next_line(int fd, char **line);</code> </td>
  </tr>
  <tr>
    <td> <b>Return value</b> </td> <td> <code>1</code> :  A line has been read <br>
                                        <code>0</code> :  EOF has been reached <br>
                                        <code>-1</code> :  An error happened   </td>
  </tr>
  <tr>
    <td> <b>Preprocessor definition</b> </td> <td> <code>-D BUFFER_SIZE=_your_val_;</code> 32 by default</td>
  </tr>
  <tr>
    <td> <b>Binary file reading</b> </td> <td>Not Supported</td>
  </tr>
    <tr>
    <td> <b>Multiple fd reading</b> </td> <td>Supported</td>
  </tr>
</table>

`get_next_line()` has an undefined behavior if, between two calls,the same file descriptor switches to a different file before EOF has been reached onthe first fd.
