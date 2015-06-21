# assignment2
makeCacheMatrix <- function(x = matrix()) {
   m <- NULL
   set <- function(y){
       x <<- y
       m <<- NULL
}
   get <- function() x
   setmatrix <- function(inverse) m <<- inverse
   getinverse <- function()m

   list(set = set,
   get = ,
   setinverse = setinverse,
   getinverse = getinverse)
}
cacheSolve <- function (x=matrix(),...){
m<-x$getinverse(){
if(!is.null(m)){
if(x$setmatrix() == x$getmatrix()){
return(m)
}
y<-x$getmatrix()
x$setmatrix(y)
m<- solve(y, ...)
x$setinverse(m)
m
