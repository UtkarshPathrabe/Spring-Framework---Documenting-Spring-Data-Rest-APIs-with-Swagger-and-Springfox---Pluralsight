Spring Framework: Documenting Spring Data Rest APIs with Swagger and Springfox  
==============================================================================  

Q01. Which option makes it easiest to use an API?  
A. No documentation  
B. Old documentation  
C. Current documentation  
D. Incorrect documentation  
Answer: `Current documentation`  

Q02. What is Swagger?  
A. Another name for Springfox  
B. A browser-based REST client  
C. An API specification and a set of tools for working with APIs  
D. A company that creates documentation tools  
Answer: `An API specification and a set of tools for working with APIs`  

Q03. What is the name of the object you use to configure Swagger?  
A. ApiInfo  
B. Document  
C. Docket  
D. Docker  
Answer: `Docket`  

Q04. Why would you use Springfox in a Spring Data REST API project instead of using Swagger directly?  
A. Springfox interprets Spring annotations for Swagger information so you don't have to annotate everything.  
B. Springfox helps you manage multiple versions of your API.  
C. Springfox is the only way to customize the Swagger UI.  
D. Springfox maintains the open source code for the Swagger UI.  
Answer: `Springfox interprets Spring annotations for Swagger information so you don't have to annotate everything.`  

Q05. When might you define more than one Docket object in a project?  
A. To partition documentation by version  
B. If you have more than one entity  
C. To use different Springfox libraries  
D. You can only define one Docket object  
Answer: `To partition documentation by version`  

Q06. Given the following code, what, if anything, needs to be modified for a red `*` (asterisk) to appear next to `name` in the Swagger UI?  
```
@ApiModelProperty(value = "Customer facing name")
@NotNull
public String name;
```  
A. Add `required=true` to `@ApiModelProperty`  
B. Remove the `@NotNull` annotation  
C. Add a `@Required` annotation to `name`  
D. The code as shown is correct. NO changes are needed.  
Answer: Add `required=true` to `@ApiModelProperty`  

Q07. If you want to partition your documentation, what property do you need to set?  
A. `groupName` in `Docket`  
B. `@EnableSwagger2WebMvc` on your configuration class  
C. `apiInfo` in `Docket`  
D. `@ApiOperation` on every method  
Answer: `groupName` in `Docket`  

Q08. If you want to add additional information about entity values and have it displayed in the Swagger UI, what annotation do you need to use?  
A. @ApiOperation  
B. @ApiModelProperty  
C. @EntityValue  
D. @ApiValue  
Answer: `@ApiModelProperty`  

Q09. If you have a class named "Employee" and a property named "name", which option adds value to the documentation?  
A.  
```
public class Employee {
  @ApiModelProperty(value="First and last name")
  public String name;
```  
B.  
```
public class Employee {
  @ApiModelProperty(value="Employee name")
  public String name;
```  
C.  
```
public class Employee {
  public String name;
```  
D.  
```
public class Employee {
  @ApiModelProperty(value="Name of Employee")
  public String name;
```  
Answer:  
```
public class Employee {
  @ApiModelProperty(value="First and last name")
  public String name;
```  

Q10. What object do you need to modify if you want to change API level attributes in the Swagger UI? For example, title, version, description.  
A. Docket  
B. ApiProperties  
C. SwaggerConfig  
D. ApiInfo  
Answer: `ApiInfo`  