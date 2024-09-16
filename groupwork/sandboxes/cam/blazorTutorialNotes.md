# Blazor tutorial Notes
## https://learn.microsoft.com/en-ca/training/paths/build-web-apps-with-blazor/

### Create and run a new Project 
Open a terminal in vsCode\
Navigate to the folder where you would like to create a project\
- Run the following command, replace testApp with desired name\
dotnet new blazorwasm -o testApp\
- run the following command to launch the app in your browser
dotnet watch\

###Enable interactivity
To handle UI events from a component and to use data binding, the component must be\ interactive. By default, Blazor components render statically from the server, which means\ they generate HTML in response to requests and are otherwise unable to handle UI events.\ You make a component interactive by applying an interactive render mode using the\ @rendermode directive.\

You can apply the @rendermode directive to a component definition:\
@rendermode InteractiveServer\

Or to a component instance:\
<Counter @rendermode="InteractiveServer" />\

Alternatively, Blazor components can use the InteractiveWebAssembly render mode to render\ interactively from the client. In this mode, the component code is downloaded to the\ browser and run client-side using a WebAssembly-based .NET runtime.\

### Info on Render modes 
https://learn.microsoft.com/en-us/aspnet/core/blazor/components/render-modes?view=aspnetcore-8.0\

### Random syntax to remember 
The name of a Blazor component must begin with an uppercase character\

