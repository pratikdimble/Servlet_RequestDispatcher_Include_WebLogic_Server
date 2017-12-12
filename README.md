# Servlet_RequestDispatcher_Include

The RequestDispatcher interface provides the facility of dispatching the request to another resource it may be html,servlet or jsp.
This interface can also be used to include the content of another resource also. 
It is one of the way of servlet collaboration. 
------------------------------------------------------------------------------------------------------------
There are two methods defined in the RequestDispatcher interface.

# Methods of RequestDispatcher interface

The RequestDispatcher interface provides two methods. They are:
   # 1. public void forward(ServletRequest request,ServletResponse response)throws ServletException,java.io.IOException:
    Forwards a request from a servlet to another resource (servlet, JSP file, or HTML file) on the server.
    
    # 2. public void include(ServletRequest request,ServletResponse response)throws ServletException,java.io.IOException:
    Includes the content of a resource (servlet, JSP page, or HTML file) in the response.
---------------------------------------
# How to get the object of RequestDispatcher

The getRequestDispatcher() method of ServletRequest interface returns the object of RequestDispatcher. Syntax:
Syntax of getRequestDispatcher method

 # public RequestDispatcher getRequestDispatcher(String resource);  

Example of using getRequestDispatcher method

# RequestDispatcher rd=request.getRequestDispatcher("servlet2");

## rd.include(request, response);//method is include 

# rd.forward(request, response);//method is forward  
     
      
  

Example of RequestDispatcher interface


    addForm.html file: for getting input from the user.
    web.xml file: a deployment descriptor file that contains the information about the servlet.

