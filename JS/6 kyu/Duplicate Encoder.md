## Check out this [kata](https://www.codewars.com/kata/54b42f9314d9229fd6000d9c)

### Description:

The goal of this exercise is to convert a string to a new string where each character in the new string is 

"(" if that character appears only once in the original string, or ")" if that character appears more than once 

in the original string. Ignore capitalization when determining if a character is a duplicate.

## My Solution:
```
function duplicateEncode(word){
  const letterArray = word.toLowerCase().split("");
  let outPutString = [];
  for (i in letterArray) {
    outPutString.push(
      word.toLowerCase().split(letterArray[i]).length - 1 <= 1 ? "(" : ")"
    )
  }
  return outPutString.join("");
}
```

