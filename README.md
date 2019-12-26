# user-urls

Users have a URL that changes as they move the mouse around an application. This URL captures what else is on the screen. It represents a query for what the user is able to do right now.

# Usages

Real time search for future options.

# Examples

In a code IDE where you have the mouse cursor in a definitive position, such as the following where my cursor in inside the `index` method of a Spring boot controller:

```
package hello;

import org.springframework.web.bind.annotation.RestController;
import org.springframework.web.bind.annotation.RequestMapping;

@RestController
public class HelloController {

    @RequestMapping("/")
    public String index() {
        //my cursor is here
        return "Greetings from Spring Boot!"; 
    }

}
```
The url should look something like:
```
user://main.editor?file=HelloController.java&class=HelloController&classAnnotation=@RestController&method=index&methodAnnotation=@RequestMapping("/")
```
