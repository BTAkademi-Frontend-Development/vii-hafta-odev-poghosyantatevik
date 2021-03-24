# vii-hafta-odev

- Haftasonu yapılan todo-example örneğini geliştirmeye çalışınız.

- Array Metodlardan "Map, Filter, Reduce" ile örnekler yapmaya çalışınız.

  :dart:
  
  :triangular_flag_on_post: **Map**
  
  The map() method creates a new array with the results of calling a function for every array element.

  The map() method calls the provided function once for each element in an array, in order.

  Note: map() does not execute the function for array elements without values.

  Note: this method does not change the original array.
  
  
  **e.g.**
  
  
     let a = [12, 4, 17, 2, 18];
     
    let b = a.map(function(val) { 
    
     return val * 2;
        
    });
    
     alert(b); // in this case our answer will be [24, 8, 34, 4, 36]
     

    :triangular_flag_on_post: **Filter**
     
     The filter() method creates an array filled with all array elements that pass a test (provided as a function).

     Note: filter() does not execute the function for array elements without values.

     Note: filter() does not change the original array.
     
     
     **e.g.**
     
     
     let a = [15, 12, 37, 22, 58];
     
     let b = a.filter(function(val) {
    
     return (val % 2) === 0;
        
    });
    
     console.log(b); // in this case the result will be [12, 22, 58]

    
    :triangular_flag_on_post: **Reduce**
    
    The reduce() method reduces the array to a single value.

    The reduce() method executes a provided function for each value of the array (from left-to-right).

    The return value of the function is stored in an accumulator (result/total).
  
    Note: reduce() does not execute the function for array elements without values.

    Note: This method does not change the original array.


    **e.g.**
    
    let a = [9, 3, 5, 19].reduce(function(aggr, val) {
    
    return aggr + val;
    
    }, 0);
    
   alert(a); // the output will be 36



- OWASP Top Ten Güvenlik Kurallarını özetleyiniz.
