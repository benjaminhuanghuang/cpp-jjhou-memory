![](./_images/cpp-memory-api.png)


![](./_images/cpp-memory-api-2.png)


![](./_images/cpp-memory-sample.png)

GUN 4.9
![](./_images/cpp-memory-sample-2.png)



## new expression (VC)
![](./_images/new-expression.png)
_callnewh(size) 用于release memory when malloc() failed


## delete expression
![](./_images/delete-expression.png)

## Call constructor and distructor
实验证明不能直接调用constructor
![](./_images/ctor-dtor.png)


## array new, array delete
![](./_images/array-new-delete.png)
array new 会调用class的defult constructor, 此处无法调用带参数的contructor
![](./_images/array-new-delete-sample.png)
```
  new(obj_pointer)A(i)
```
用来调用obj_pointer处的constructor

## array size in memory block
size of memory block要是16的整数倍

![](./_images/array-memory-block.png)
对于 int array, delete 可以不用加[]

![](./_images/array-memory-block-2.png)

## placement new
