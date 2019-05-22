
You'll build a service that will accept HTTP GET requests at:


 http://&lt;server&gt;:&lt;port&gt;/greeting


and respond with a link:/understanding/JSON[JSON] representation of a greeting:

 [source,json]

 {"id":1,"content":"Hello, World!"}


You can customize the greeting with an optional `name` parameter in the query string:

 http://&lt;server&gt;:&lt;port&gt;/greeting?name=User


The `name` parameter value overrides the default value of "World" and is reflected in the response:

 [source,json]

 {"id":1,"content":"Hello, User!"}


