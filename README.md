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

 :dart: **OWASP TOP 10**
 
 Here is the official link to get more info about [OWASP](https://owasp.org/www-project-top-ten/)
 
 **1. Injection**
The first vulnerability relates to trusting user input. An injection happens when an attacker sends invalid data to the application with an intent to make the application do something that it’s ideally not supposed to do. 

**2. Broken Authentication and Session Management**
The second vulnerability covers the ability of users to manipulate, or workaround authentication mechanisms and sessions within an application. 

**3. Cross-Site Scripting (XSS)**
This vulnerability occurs at the browser-level when user data is rendered without being escaped or validated. Attackers could injection malicious scripts to retrieve sensitive information or manipulation the way the application looks.

**4. XML External Entities (XXE)**
You can find this vulnerability in applications that are poorly and insecurely processing XML data. Many applications use XML to transfer data to and from browser and servers. There are different features and specifications of XML and some of these and dangerous. Attackers can manipulate with the XML data to perform malicious tasks.

**5. Security Misconfiguration**
This vulnerability occurs when configurations have not been security hardened. As the application keeps getting complex, there’s a lot of things to take care. And if you don’t give enough attention to detail, you might end up with security misconfigurations. This vulnerability depends on the way things are built and maintained.

**6. Sensitive Data Exposure**
This vulnerability relates to any access to information by anyone who shouldn’t have access to it such as credentials, credit card details, etc. This includes data rendered in a browser or API response, data in logs and regular backups, and data sent between the client and the server.

**7. Broken Access Control**
You can find this vulnerability in web applications that have user-specific control. An application can have 3 types of users in general:

Anonymous users (users without logging in).

Normal users (logged in but have minimum privileges and functions)

Admin users

**8. Insecure Deserialization**
This vulnerability exists where the data is being serialized and deserialized. Serialization means breaking data into a form for different purposes for transfer or storage. And deserialization is putting the broken data back together. Insecure deserialization occurs when the application puts back data together without checking for maliciousness or change in data.

**9. Using Components With Known Vulnerabilities**
This vulnerability, as the name says, is where one or more components upon which an application depends, has a known vulnerability. This can include a third-party software library, a version of the web server or even in the operating system itself.

**10. Insufficient Logging & Monitoring**
Web application security is not a one-step process and doesn’t end after you implement measures. You have frequently, or even better continuously monitor your application. Insufficient logging and monitoring will stop you from identify incidents earlier before they do any real harm. You can use attack indicators and signature along with logging and monitoring to identify possible security attacks and prevent them from succeeding. This will also help you in knowing your application’s security and improving it.


