#Readme.MD for the cachematrix function.

Hello fellow learners. I am submitting my .R code file for the week 3 Programming Assignment 2.

Here's how I have tested it.

After writing the funcctions, I created a matrix x with some data.

    x <- matrix(c(1:8,-2),nrow=3,ncol=3)

    x [,1] [,2] [,3] [1,] 1 4 7 [2,] 2 5 8 [3,] 3 6 -2

Now I made a call to the makeCacheMatrix

    myVect <- makeCacheMatrix(x)

Check the expected inverse value by running

    solve(x) [,1] [,2] [,3] [1,] -1.75757576 1.5151515 -0.09090909 [2,] 0.84848485 -0.6969697 0.18181818 [3,] -0.09090909 0.1818182 -0.09090909

Calling the cacheSolve for inverse.

    cacheSolve(myVect) [,1] [,2] [,3] [1,] -1.75757576 1.5151515 -0.09090909 [2,] 0.84848485 -0.6969697 0.18181818 [3,] -0.09090909 0.1818182 -0.09090909

Second run of the same thing shows value from cache.

    cacheSolve(myVect) getting cached data [,1] [,2] [,3] [1,] -1.75757576 1.5151515 -0.09090909 [2,] 0.84848485 -0.6969697 0.18181818 [3,] -0.09090909 0.1818182 -0.09090909

