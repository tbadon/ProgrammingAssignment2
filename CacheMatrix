## Put comments here that give an overall description of what your
## functions do
        ### These functions cache the matrix and solve for the inverse of the matrix
## Write a short comment describing this function
        ### caches matrix
makeCacheMatrix <- function(x = matrix()) {
inv <- NULL                             ## inv as NULL 
  set <- function(y) {                     
    x <<- y                            
    inv <<- NULL                        ## in new matrix, reset inv to NULL
  }
  get <- function() x                     
  
  setinverse <- function(inverse) inv <<- inverse  
  getinverse <- function() inv                     
  list(set = set, get = get, setinverse = setinverse, getinverse = getinverse)
}


## Write a short comment describing this function
        ### solves for inverse of 'x'
cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
        inv <- x$getinverse()
  if(!is.null(inv)) {
    message
    return(inv)
  }
  data <- x$get()
  inv <- solve(data, ...)
  x$setinverse(inv)
  inv
}
