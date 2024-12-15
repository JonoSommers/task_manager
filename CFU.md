Define CRUD.
    - It stands for Create, Read, Update, Delete.
    - These are the four fundamental operations that can be preformed on data within a database.
    - They can create new data entries, retrieve existing data, modify existing data, and delete data.

Define MVC.
    - It stands for Model-View-Controller and is a design pattern that describes the primary responsibility of each portion of code.
    - The model handles data and logic.
    - The view handles the user interface.
    - The controller is in charge of how the model and view work together.

What two files would you need to create/modify for a Rails application to respond to a GET request to /api/v1/tasks, assuming you have a Task model.
    - You would need to create a tasks_controller.rb file inside the v1 directory, and define the logic for what should happen when a request is routed to the controller action (GET, POST, PUT/PATCH, DELETE).    
    - You would also need to modify the routes.rb file to point to the tasks_controller.rb, so that Rails knows where to route the request.

What are params? Where do they come from?
    - Params are objects in Rails that hold all the data sent with a user's request. They allow you to access the information in that request, such as IDs, form data, or JSON data.
    - Params come fome from the user data. For example if they visit a URL that ended with /tasks/1 the param would be 1 which is the ID of the task (access it by using params[:id]).

What is the purpose of a serializer?
    - They allow us to control exactly what data we send to the user from our database, how we want it formatted, and even the ability to add in additional information that may not be stored in our database.