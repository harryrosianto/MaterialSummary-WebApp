### 1. Servlet API and JSP Overview
- **Servlet**: A Java program that runs on a server, handling client requests and generating dynamic web content.
- **Servlet API**: Provides the necessary interfaces and classes for writing servlets. Key components include `HttpServlet`, `HttpServletRequest`, `HttpServletResponse`, and the servlet lifecycle methods (`init`, `service`, `destroy`).

### 2. JSP Elements and Components
- **JSP Page Elements**:
  - **Directives**: `<%@ %>` used for setting up the page environment, such as `<%@ page %>`, `<%@ include %>`, and `<%@ taglib %>`.
  - **Declarations**: `<%! %>` for declaring variables and methods.
  - **Scriptlets**: `<% %>` for embedding Java code.
  - **Expressions**: `<%= %>` for outputting values.
  - **Actions**: `<jsp:action>` tags for performing built-in functionalities like `<jsp:include>`, `<jsp:forward>`, and `<jsp:useBean>`.
  - **Implicit Objects**: Predefined variables like `request`, `response`, `session`, `application`, `out`, `config`, `pageContext`, `page`, and `exception`.

### 3. JSP Actions and Implicit Objects
- **JSP Actions**: Tags that perform built-in functions, such as `jsp:include`, `jsp:forward`, and `jsp:useBean`.
- **Implicit Objects**: Objects available in JSP pages without explicit declaration, such as `request`, `response`, `session`, `application`, `out`, `config`, `pageContext`, `page`, and `exception`.

### 4. JSP Standard Tag Library (JSTL)
- **JSTL**: A collection of tags that provide core functionalities, such as loops and conditionals. Categories include:
  - **Core Tags**: General-purpose tags.
  - **Formatting Tags**: For formatting text, dates, numbers.
  - **SQL Tags**: For interacting with databases.
  - **XML Tags**: For manipulating XML data.

### 5. HTTP Protocol
- **HTTP Requests**: Consist of methods like GET, POST, PUT, DELETE, headers, and body content.
- **HTTP Responses**: Include status codes, headers, and body content. Notable status codes include 200 (OK), 404 (Not Found), 500 (Internal Server Error).

### 6. Web Architecture and Components
- **Web Server**: Delivers web pages, images, and other resources over the web.
- **Tiers in Web Applications**: Logical chunks such as presentation tier, logic tier, and data tier.

### 7. Cookies in Servlets
- **Creating Cookies**: Use `new Cookie(name, value)` and `setMaxAge(seconds)` to set the expiration.
- **Retrieving Cookies**: Use `request.getCookies()` and iterate to find the desired cookie.

### 8. Expression Language (EL)
- **EL Implicit Objects**: Objects like `param`, `paramValues`, `header`, `headerValues`, `cookie`, and `initParam`.

### 9. JSP and Servlet Lifecycle
- **JSP Lifecycle Methods**: `jspInit()`, `_jspService()`, and `jspDestroy()`.
- **Servlet Lifecycle**: 
  - **Class Loaded**: Servlet class is loaded.
  - **Instantiation**: Servlet instance is created.
  - **Initialization**: `init()` method is called.
  - **Service**: `service()` method handles requests.
  - **Destruction**: `destroy()` method is called before servlet is taken out of service.

### 10. Code Snippets and Examples
- **JSP `c:set` Tag**: `<c:set var="FirstNum" value="10"/>`, `<c:set var="SecondNum" value="40"/>`
- **Output with `c:out`**: `<c:out value="${FirstNum + SecondNum}"/>`

### 11. Struts Framework
- **ActionForm Bean**: Used in Struts to encapsulate form data.
- **Struts Configuration**: Registering ActionForm classes in `struts-config.xml`.
