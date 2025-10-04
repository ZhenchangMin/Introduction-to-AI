# Lec5: Trees, Minimax, Pruning
## Recap: Random restarts, parallel search and beam search
![1759593680516](image/lec5/1759593680516.png)
At first we start at 8, and get a local maximum 9.
We might think it's not so great, so we do another random restart, in yellow color, and getting a local maximum 10.
![1759593757496](image/lec5/1759593757496.png)
So by doing lots of random restarts, we have a large probability to get a global maximum, and this is parallel search.

While in beam search, the random starts communicate with each other, and get the best one.
![1759593968064](image/lec5/1759593968064.png)
Like in this case, the dark blue random start is disposed, as we only need top k best ones.

## Local Search in Continuous Space
![1759595167630](image/lec5/1759595167630.png)
Say that we're going to place 3 airports in Romania to minimize the total distance between the cities and the nearest airports.

