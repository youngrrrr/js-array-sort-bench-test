Check out my question on StackOverflow: http://stackoverflow.com/questions/34476963/why-do-arrays-of-objects-fewer-data-sort-faster-than-arrays-of-numbers-more-da

###Results from manual bench testing:

#sparseArray:
* (24 + 23 + 21 + 23 + 21 + 22 + 22 + 22 + 22 + 22 + 21 + 20 + 22 + 24 + 24 + 21 + 22 + 22 + 25 + 23 + 24 + 23 + 21 + 21 + 23) / 25 = 22.32ms

#sparseArray2:
* (4 + 4 + 4 + 4 + 4 + 5 + 5 + 5 + 5 + 4 + 6 + 5 + 5 + 4 + 5 + 4 + 4 + 4 + 5 + 6 + 4 + 5 + 4 + 4 + 5) / 25 = 4.56ms

#denseArray:
* (5 + 5 + 4 + 5 + 5 + 5 + 5 + 5 + 5 + 6 + 5 + 5 + 4 + 4 + 5 + 5 + 5 + 4 + 5 + 5 + 6 + 5 + 5 + 5 + 4) / 25 = 4.88ms

###Try it yourself:

`node arraySortTest.js`
