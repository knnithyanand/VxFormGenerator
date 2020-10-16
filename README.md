# VxFormGenerator

The library contains a component that nests itself in the Blazor EditForm. The component is able to generate a form based on a POCO or a ExpandoObject. Allowing these two methods, provides the developer with flexibility in usage. 

### Setup

Add the NuGet package.

Open a terminal in the project folder where you want to add the **VxFormGenerator**. Pick one of the options below:

###### Plain components

The unstyled version of the input components for the **VxFormGenerator**

`dotnet add package VxFormGenerator.Components.Plain`

###### Bootstrap components

The Bootstrap styled form components for the **VxFormGenerator**

`dotnet add package VxFormGenerator.Components.Bootstrap`

### Initialize

Open the `Startup.cs` and add one of the following usage statements:

###### Plain components

`using VxFormGenerator.Settings.Plain;`

###### Bootstrap components

`using VxFormGenerator.Settings.Bootstrap;`

After adding one of the usage statements add the line `services.AddVxFormGenerator();` like shown here below.

````C#
public IConfiguration Configuration { get; }

// This method gets called by the runtime. 
// Use this method to add services to the container.
// For more information on how to configure your application, 
// visit https://go.microsoft.com/fwlink/?LinkID=398940
public void ConfigureServices(IServiceCollection services)
{
	services.AddRazorPages();
	services.AddServerSideBlazor();
	services.AddVxFormGenerator();
}
````



### Model based

You can have a model that renders inputs for the properties. The inputs can be validated by the attached DataAnotations on the property.







### Dynamic based



