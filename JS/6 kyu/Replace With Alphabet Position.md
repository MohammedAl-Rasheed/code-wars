## Check out this [kata](https://www.codewars.com/kata/546f922b54af40e1e90001da)

### Description:

In this kata you are required to, given a string, replace every letter with its position in the alphabet.

If anything in the text isn't a letter, ignore it and don't return it.

"a" = 1, "b" = 2, etc.

## My Solution:
```
function alphabetPosition(text) {
  var result= "";
  for (var i = 0; i < text.length; i++) {
    var code = text.toUpperCase().charCodeAt(i)
    if (code > 64 && code < 91) result += (code - 64) + " ";
  }
  
  return result.slice(0, result.length - 1);
}
console.log(alphabetPosition("The sunset sets at twelve o' clock."));
};
```


