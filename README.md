[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
mystery() takes a list of numbers as an argument, then, provided the length of the list is > 1, recursively slices the array down to the last element 
and adds that to the foo variable. Then it compares foo to the first element of the orignal array, and returns the greater of the two. The return value is the 
maximum value of all the elements in the orignal array.. If the length of the list is 1, it returns that element. 
