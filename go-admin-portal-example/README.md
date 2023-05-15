# Go Admin Portal Example

An example Golang application demonstrating how to use the [WorkOS Golang SDK](https://github.com/workos/workos-go) so your customers can access the WorkOS Admin Portal from your application.

## Go Project Setup

1. Clone the example repository using your preferred secure method (HTTPS or SSH).

   ```bash
   # HTTPS
   git clone https://github.com/workos/go-example-applications.git
   ```

   or

   ```bash
   # SSH
   git clone git@github.com:workos/go-example-applications.git
   ```

2. Navigate to the cloned repository and to the admin portal:

   ```bash
   cd go-example-applications/go-admin-portal
   ```

3. Obtain and make note of the following values. In the next step, these will be set as environment variables.

   - Your [WorkOS API key](https://dashboard.workos.com/api-keys)

4. Create a new file called ".env" in the root of the project and add the following variables, replacing the xxx with the value from step 3:
   - WORKOS_API_KEY=xxx

## Start the server

5. The final setup step is to start the server.

   ```bash
   go run main.go
   ```

   You'll know the server is running when you see no errors in the CLI, and output similar to the following is displayed:

   ```bash
   launching admin portal demo with configuration: {Addr::8000 Domains:}
   ```

   Navigate to `localhost:8000` in your web browser to view the homepage of the Admin Portal example app. Enter the name of the new Organization to be created and the names of all of the Organization's associated domains.

   - The Organization must be a new Organization that doesn't yet exist in your WorkOS dashboard
   - The domains should be entered as space-separated values, e.g. "domain1.com domain2.com domain3.com"

Then, click the buttons to either create a new SSO connection or a new Directory Sync connection. Hooray!

## Need help?

If you get stuck and aren't able to resolve the issue by reading our API reference or tutorials, you can reach out to us at support@workos.com and we'll lend a hand.
