

function beggars(values, n){
  var totals = []
  for (var i = 1; i <= n; i++) {
    var sum = 0
    for (var j = i; j <= values.length ; j += n) {
      sum += values[j - 1]
    }
    totals.push(sum)
   }
   return totals
}
