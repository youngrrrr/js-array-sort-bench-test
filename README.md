Check out my question on StackOverflow: http://stackoverflow.com/questions/34476963/why-do-arrays-of-objects-fewer-data-sort-faster-than-arrays-of-numbers-more-da

#Results from manual bench testing:

###sparseArray:
* (4+4+4+4+3+4+4+4+4+4+4+4+3+4+4)/15 = 3.867ms

###sparseArray2:
* (4+4+4+6+5+4+4+4+4+5+5+4+5+5+5)/15 = 4.533ms

###denseArray:
* (4+4+4+5+5+4+4+4+4+5+5+4+5+5+5)/15 = 4.466ms

#Try it yourself:

`node arraySortTest.js`

#Notes:

I don't really know if my implementation of testing is super accurate. For some reason, the very first test seems to be much slower than subsequent ones. This is why I added a 'buffer' array for the sorting. There may also be other biases stemming from the order in which the tests are run, so I tried to account for that in the results by switching up the order on a per-trial basis.