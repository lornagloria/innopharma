# innopharma 
Usage and Testing READmd
This section details the basic steps to access and verify the core functionality of the running pharmacy tracking system(innopharma).
How to Run and Access
 * Open the Web App: Once the front-end (React) server is running, access the main interface at:
   http://localhost:3000

 * Verify Backend Connection: The home screen should successfully load initial medication data from the API endpoint.
Basic Usage Examples
1. Checking the API Status
Use a browser or a tool like Postman/cURL to confirm the Node.js server is online and responding:
# Check if the server's pharmacy endpoint is reachable
curl http://localhost:5000/api/status 

(The expected response should be a JSON object like {"status": "API running"})
2. Adding a New Record
Navigate to the "New Admission" page and submit a new patient entry. Verify that the new data appears in the main patient list view.
Running Tests
Execute the automated tests located in the server directory to ensure all back-end functions (like data validation and API routes) are stable:
cd server
npm test

(This command runs all unit tests defined in the server code.)