# AspWebApplication

**In this app we used to pratice on the CRUD function inside the web.**

## Steps:

1- Create a ASP.NET Core project with an Entity Framework using MVC design pattern.








## Endpoints
**Endpoints are the app units of executable request handler code. Endpints are defined in the app and configured when the app start. So the endpoints matching process can extract values from the requested URL and provide those values for requested processing. Using endpoints information from the app rooting us also able to generate URL's that map to the endpoints**  
1- MVC
2- Razor Pages
3- SignalR

## Routing 

1- **Conventional-Based Routing:**
  The route is determined based on the rules defined in the route template
  i.e. http://localhost:40268/student/index/
    first segment is domain name localhost:40268
    second segment is controller student
    third segment is action index
2- **Attribute-Based Routing:**
  The route is determined based on the attributes configured at the controller level or the action method level
  i.e.  http://localhost:40268/student/index/id
  ```
  public class StudentController : Controller
    {
        StudentContext std = new StudentContext();

        //  http://localhost:40268/student/index/id 
        [Route("Student")]
        [Route("Student/Index")]
        [Route("Student/Index/{id}?")]
        public IActionResult Index()
        {
            return View();
        }
     }
     
   ```     
   
   # Controller Actions
   
   controller action are the methods udes to handle the HTTP requests and act accordingly to return the view or other results.
   
   ## Action
   
   Actions are the methods in the controller class that are responsible for the returning the view or JSON data.
   Any public method on a controller type is an action
   Any public methods are created inside the controller class is a type of action
   
   ## Action Results
   
   A result of action methods or return types of action methods 
   
   ## Action methods cannot be overloaded 
   
   ## Action methods cannot be  static
   
   ``` 
   public IActionResult details(int id)
    {
        return Ok("You have entered the ID = " + id);
    }
  ```
  ## Action Results
  *Types of action results*
  1- Status Code results
  2- 
  ### Return-Type : 
  interface => IActionResult
  ### ActionResult
  abstract class from different action are inherited
  
  ## Action Parameters  (Pass values to actions)
  
  ## Action Results
  these are the classes which represents things the client is supposed to do as a result of the controller.
  
  # Models
  
  shape of the data
  domain specific and business logic MVC architecture 
  maintains the data of the application
  
  
  
  # Code First Approach and Migration
  
  
  # MIGRATION
  
  
   
   
