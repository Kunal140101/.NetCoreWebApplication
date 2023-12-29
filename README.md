To run the application first open the "Package Manager Console" and run the command 'dotnet restore' to restore the NuGet packages.
On selecting the 'Build' tab click on 'build solution'
Then to run the application set the startup project to Galytix.WebApi (right-click on the project in Solution Explorer -> Set as Startup Project) and press F5 or click on the "Start Debugging" button to run the application.
Verify Console Output
Open your web browser and navigate to http://localhost:9091/swagger. This opens the Swagger UI, allowing you to explore and test the available API endpoints.
Test the CountryGwp Endpoint:

In Postman or any API testing tool, create a new POST request to http://localhost:9091/api/CountryGwp/avg.
Set the request body to the following JSON payload:
{
    "country": "ae",
    "lob": ["property", "transport"]
}
Send the request and verify the response. The response should include the calculated averages for the specified country and lines of business
