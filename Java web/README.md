# [MODULE-1] Audit Module 2 - Javaweb

##Nội dung câu hỏi và phần trả lời

## [ Câu hỏi ] 1.  What is Webservice?
```
- method of communication between two electronic devices over the World Wide Web
```
## [ Câu hỏi ] 2.  What project did you use Webservice for?
```
```
## [ Câu hỏi ] 3.  What function did you Webservice provide?
```
```
## [ Câu hỏi ] 4.  What server did you use to run?
```
```
## [ Câu hỏi ] 5.  How did you test your Webservice?
```
- RESTful client (add-on of Firefox)
- SOAP UI
```
## [ Câu hỏi ] 6.  What do you use to parse JSON data?
```
- Use Json or Jackson libraries
- Create JSONObject (Please check sample code to see the details)
```
## [ Câu hỏi ] 7.  How do you read XML file using JAXB?
```
a. Create POJO with annotations
b. Create JAXBContext
c. Create a marshaller or an unmarshaller to convert
d. Please check sample code to see the details 
```
## [ Câu hỏi ] 8.  How would you write a simple REST client?
```
- Using Jersey:
o Create client config
o Create client
o Get resource for client from URI
o Getting data by path and media type/ posting data
```
## [ Câu hỏi ] 9.  How do you get the parameter in Restful?
```
- Jersey: pathParam, QueryString
- Spring MVC: @PathVariable
```
## [ Câu hỏi ] 10.  What XML Binding tool do you use?
```
- JAXB
```
## [ Câu hỏi ] 11. What are the differences between SOAP and REST?
```
- Architecture:
o SOAP: XML-based message protocol
o REST: architectural style
- Communication:
o SOAP: WSDL
o REST: XML + JSON (WADL)
- Invocation:
o SOAP: RPC method
o REST: URL path
- Returned result:
o SOAP: doesn’t return human readable
o REST: return human readable (XML + JSON)
- Protocol:
o SOAP: HTTP, SMTP, FTP…
o REST: HTTP
```
## [ Câu hỏi ] 12. What is JAX-RS, and why did you use it ?
```
- Java API for RESTful webservice
- Support to create RESTful webservice
```
## [ Câu hỏi ] 13. What JAX-RS implementation did you use ?
```
- Jersey
- Spring MVC
```
## [ Câu hỏi ] 14. Could you explain about WADL?
```
- Web Application Description Language
- Machine-readable XML of HTTP-based web application
- Models resources, relationship, methods applied, representation format
```
## [ Câu hỏi ] 15. Have you worked with consuming or producing Web Service?
```
- Both
- Jersey Client + Jersey
```
## [ Câu hỏi ] 16. Can you explain about WSDL?
```
- Webservice Description Language
- XML-based interface for describing function
```
## [ Câu hỏi ] 17. What are different states of object in Hibernate?
```
- Transient: not associated with persistence context
- Persistence: associated with persistence context
- Detached: not associated with because persistence context is closed
```
## [ Câu hỏi ] 18. What is the meaning of the Controller annotation?
```
- To identify that class acts as a controller
```
## [ Câu hỏi ] 19. What is Spring?
```
- Open source framework, light weight
- Layer architecture
- Support java enterprise application
```
## [ Câu hỏi ] 20. What are features of Spring?
```
- Lightweight
- IOC
- AOP
- Container
- MVC
- Transaction management
- JDBC Exception Handling
```
## [ Câu hỏi ] 21. What is IOC? Dependency Injection?
```
- IOC:
o Inversion of Control
o Invert control of creating object from new operator to container 
- DI:
o Dependency Injection
o Implementation of IOC
o All dependencies of an object are injected into it by framework
```
## [ Câu hỏi ] 22. What is AOP?
```
- Aspect Oriented Programming
- Modularizes cross-cutting concerns (logging, security, transaction management..)
```
## [ Câu hỏi ] 23. Explain Aspect, Advice, Joint Point, Pointcut?
```
- Aspect:
o a modularization of a concern
o cuts across multiple classes
o Eg: transaction management
- Join point:
o a point during the execution of a program
o in Spring AOP: represents a method execution
- Advice:
o action taken by an aspect at a particular join point
o Different types: around, before and after advice
- Pointcut:
o Collection of Joint Points
```
## [ Câu hỏi ] 24. What are different types of DI?

```
- Constructor injection
- Setter injection
- Interface injection
- Spring support Constructor Injection & Setter Injection
```
## [ Câu hỏi ] 25 What are the benefits of DI?
```
- Minimize amount of code
- Make application more testable
- Loose coupling
- Eager instatiation + lazy loading
- Flexible, security
```
## [ Câu hỏi ] 26. Could you decribe the life cycle of Spring beans?
```
- Bean Container finds definition of bean
- Create a instance of bean
- Depending on the interface, the properties of the bean ->  setter method will be called
```
## [ Câu hỏi ] 27. What is BeanFactory?
```
- Base on Factory pattern and IOC design
- Support 2 bean scopes: singleton + prototype
```
## [ Câu hỏi ] 28. What is ApplicationContext? What is the different between BeanFactory and ApplicationContext?
```
- ApplicationContext  Derives from BeanFactory
- Has all functionality of BeanFactory + support:
o Internationalization messsages
o Many enterprise service(EJB, JNDI…) 
o Access to resource (URL + file)
o Application life-cycle events
o Publish events to bean registered as listenter
o Loading mutiple context
```
## [ Câu hỏi ] 29. How many types of bean scopes supported  by Spring? And explain them.
```
- 5 types:
o Singleton: default scope of Spring, 1 object instance per Spring container
o Prototype: new object is created + returned whenever you get the bean
o Request: new object for each HTTP request
o Session: new session is created -> new instance object of bean
o Global session: same as HTTP session scope, applicable in portlet-based web app
```
## [ Câu hỏi ] 30. Sự khác nhau giữa 2 phương thức Get và Post.
```
- Điểm chung: là các HTTP method dùng để trao đổi dữ liệu giữa client và server.
- Điểm khác nhau:
o POST: Bảo mật hơn GET vì dữ liệu được gửi ngầm, không xuất hiện trên URL
o GET: Dữ liệu được gửi tường minh, chúng ta có thể nhìn thấy trên URL, đây là lý do khiến nó không bảo mật so với POST.
o GET thực thi nhanh hơn POST vì những dữ liệu gủi đi luôn được webbrowser cached lại.
o Khi dùng phương thức POST thì server luôn thực thi và trả về kết quả cho client, còn phương thức GET ứng với cùng một yêu cầu đó webbrowser sẽ xem trong cached có kết quả tương ứng với yêu cầu đó không và trả về ngay không cần phải thực thi các yêu cầu đó ở phía server.
o Đối với những dữ liệu luôn được thay đổi thì chúng ta nên sử dụng phương thức POST, còn dữ liệu ít thay đổi chúng ta dùng phương thức GET để truy xuất và xử lý nhanh hơn.Quan
```
## [ Câu hỏi ] 31. Mô hình MVC là gì.
```
Mô hình MVC (Model – View – Controller) là một kiến trúc phần mềm hay mô hình thiết kế được sử dụng trong kỹ thuật phần mềm. Nó giúp cho các developer tách ứng dụng của họ ra 3 thành phần khác nhau Model, View và Controller. Mỗi thành phần có một nhiệm vụ riêng biệt và độc lập với các thành phần khác
```
## [ Câu hỏi ] 32. Dependency Injection và IoC là gì.
```
- Inversion of Control: Đây là một design pattern được tạo ra để code có thể tuân thủ nguyên lý Dependency Inversion. Có nhiều cách hiện thực pattern này: ServiceLocator, Event, Delegate, … Dependency Injection là một trong các cách đó.
- Dependency Injection: Đây là một cách để hiện thực Inversion of Control Pattern (Có thể coi nó là một design pattern riêng cũng được). Các module phụ thuộc (dependency) sẽ được inject vào module cấp cao.
```
## [ Câu hỏi ] 33. Cơ chế hoạt động của FrontController trong Spring.
```
Tất cả các request phải đi qua Front-controller, front controller sẽ đưa request đến Controller phù hợp cũng như đưa dữ liệu đến view phù hợp
```
## [ Câu hỏi ] 34. Các cách để nhận dữ liệu từ view trong  Spring controller.
```
@RequestMapping, @PathVariable, @ModelAttribute...
```
## [ Câu hỏi ] 35. Databinding trong Spring?.
```
Giải thích rõ về cách controller đưa object xuống view để nhận dữ liệu
```
## [ Câu hỏi ] 36. ORM là gì?.
```
Object Relation Mapping
```
## [ Câu hỏi ] 37. Phân biệt Session và cookie.
```
- Cookie
o Dữ liệu cookie được lưu trữ ở phía client.
o Dữ liệu cookie dễ dàng sửa đổi hoặc đánh cắp khi chúng được lưu trữ ở phía client.
o Dữ liệu cookie có sẵn trong trình duyệt đến khi expired.
- Session
o Dữ liệu session được lưu trữ ở phía server.
o Dữ liệu session không dễ dàng sửa đổi vì chúng được lưu trữ ở phía máy chủ.
o Sau khi đóng trình duyệt sẽ hết phiên làm việc (session)
```
## [ Câu hỏi ] 38. Phân biệt @NotNull, @NotEmpty, @NotBlank trong Spring Validation.
```
Dựa vào giá trị nhận được từ ô input là null, rỗng, hay "   "
```
## [ Câu hỏi ] 39. Spring Sercurity hoạt động như thế nào.
```
Giải thích cách xác thực, cách nhận dữ liệu từ đâu để xác thực, cách config để Spring sercurity làm việc
```
## [ Câu hỏi ] 40. Formatter và Converter dùng để làm gì.
```
Dùng để chuyển đổi dữ liệu từ ô input sang kiểu dữ liệu phù hợp với đối tượng
```

## Mục tiêu

* Audit module 2 Java Web

## Youtube Link

* [[Java web] Tạo ứng dụng servlet](https://www.youtube.com/watch?v=daE0pnE_Q3s&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI)
* [[Java web] Tạo ứng dụng JSP](youtube.com/watch?v=In9-boiTd88&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=2)
* [[Java web] Tạo ứng dụng CRUD servlet, Jsp, Jstl](https://www.youtube.com/watch?v=2vH1gTiwOI0&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=8)
* [[Java web] Tổng quan về Spring MVC](https://www.youtube.com/watch?v=7Wpi_jC8CqA&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=15)
* [[Java web] DI](https://youtu.be/2BfSQhBNhkY)
* [[Java web] Jsp form Binding](https://youtu.be/Llm_Sxg_2Qg)
* [[Java web] Tạo Spring MVC bằng Intelliji](https://www.youtube.com/watch?v=M9Aze3quBKU&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=3)
* [[Java web] Tạo Project với SpringBoot](https://www.youtube.com/watch?v=tgK0kZCr8mo&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=4)
* [[Java web] Sử dụng Thymeleaf](https://www.youtube.com/watch?v=-YCd6W_UVcg&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=5)
* [[Java web] Tạo demo ModelAndView](https://www.youtube.com/watch?v=vaQxJlfmB6s&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=6)
* [[Java web] Path variables và Request Param](https://www.youtube.com/watch?v=luc3zTLri6M&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=7)
* [[Java web] View Resolver](https://www.youtube.com/watch?v=kL41e8MYrww&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=12)
* [[Java web] Cách dùng POST, GET, PUT, DELETE với Thymeleaf](https://drive.google.com/open?id=1nYtEPrC7SZSjIjEyPnFZbtbLUSQIIQ13)
* [[Java web] Cách dùng POST, GET, PUT, DELETE vơi postman](https://drive.google.com/open?id=1kxbTDPEqmvo1eqI26mUn-h3wjUzx70mV)
* [[Java web] Spring Data Binding](https://www.youtube.com/watch?v=SBbOjbIb-UU&list=PL9yu4ScFhKGyo0bRNxay5QiBTInV_mTPI&index=11)
* [[Java web] Sử dụng Entity Manager query DB](https://www.youtube.com/watch?v=BfjweILUCHs&feature=youtu.be)
* [[Java web] Session and Cookies](https://www.youtube.com/watch?v=ym4-rU9R6fM&feature=youtu.be)
* [[CaseStudy] Java web with Spring](https://www.youtube.com/watch?v=h3eeQvt9X98&list=PL9yu4ScFhKGw6mm6DMtLQ7NodYOd4xz4d)
* [[Java web] Spring Security](https://youtu.be/WNfuVJptPnQ)
* [[Java web] i18n](https://youtu.be/cfb2J8qx3Ww)
