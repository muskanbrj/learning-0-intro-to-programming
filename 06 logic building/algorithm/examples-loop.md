# Loops

## Components of a loop

1. initialization
1. condition
1. updation

## Syntax

### while-end while
```
[initialization]
while <condition> repeat
[statements]
[updation]
end while
```

### for-end for
```
for var = <range> repeat
[statements]
end for
```

## Examples

<table>

<tr>
<th>Problem</th>
<th>Algorithm</th>
</tr>

<tr>
<td>Print table of 2</td>
<td>

1. for `i = 1 to 10` loop
1. print `i * 2`
1. End for
1. Stop

</td>
</tr>

<tr>
<td>Calculate factorial of a number</td>
<td>

1. Let `n` be a number
1. Read `n`
1. Let `f` be `1` and `i` be `1`
1. While `i <= n` loop
1. `f = f * i`
1. `i = i + 1`
1. End while
1. Display `f`
1. Stop

</td>
</tr>

<tr>
<td>Print fibonacci series upto N terms</td>
<td>

1. Let `N` be a number
1. Read `N`
1. Let `a` be `0`, `b` be `1`, `c` be `1` and `i` be `3`
1. if `N >= 1` then
1. print 0
1. end if
1. if `N >= 2` then
1. print 1
1. end if
1. While `i <= N` loop
1. `c = a + b`
1. print `c`
1. `a = b`
1. `b = c`
1. `i = i + 1`
1. End while
1. Stop

</td>
</tr>

<tr>
<td>Print sum of digits of a number</td>
<td>

1. Let `N` be a number
1. Read `N`
1. Let `sum` be `0`
1. While `N > 0` loop
1. Let `d = N % 10`
1. `sum = sum + d`
1. `N = N / 10`
1. End while
1. print `sum`
1. Stop

</td>
</tr>

<tr>
<td>Print sum of square of digits of a number</td>
<td>

1. Let `N` be a number
1. Read `N`
1. Let `sum` be `0`
1. While `N > 0` loop
1. Let `d = N % 10`
1. `sum = sum + (d * d)`
1. `N = N / 10`
1. End while
1. print `sum`
1. Stop

</td>
</tr>

<tr>
<td>Print reverse of a number</td>
<td>

1. Let `N` be a number
1. Read `N`
1. While `N > 0` loop
1. Let `d = N % 10`
1. print `d`
1. `N = N / 10`
1. End while
1. Stop

</td>
</tr>

<tr>
<td>Print square of reverse of a number</td>
<td>

1. Let `N` be a number
1. Read `N`
1. Let `r = 0`
1. While `N > 0` loop
1. Let `d = N % 10`
1. `r = (r * 10) + d`
1. `N = N / 10`
1. End while
1. print `r * r`
1. Stop

</td>
</tr>

</table>

