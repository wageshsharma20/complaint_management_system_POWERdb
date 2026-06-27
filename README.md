# Complaint Management System using JsonPowerDB

## Title of the Project
Complaint Management System

## Description
This is a simple Web-based Complaint Management System built using HTML, CSS (Bootstrap), JavaScript, and **JsonPowerDB**. It allows users to register complaints, which are securely and asynchronously saved into the JsonPowerDB backend using AJAX `PUT` requests without reloading the page.

## Benefits of using JsonPowerDB
- **Nimble, Simple to use, In Memory, Real-time DBMS.**
- **Schema-free:** Easy to develop and maintain since we don't have to pre-define the schema.
- **Serverless support:** Simplifies backend development and cuts time to market.
- **Multi-mode Database:** Supports Document DB, Key-Value DB, RDBMS, and more.
- **Fastest Indexing Engine:** Built around PowerIndex, ensuring maximum data processing performance.
- **Webservices API:** Low development cost as it operates entirely via REST APIs.

## Release History
- **v1.0.0 (Current)** - Initial release of the Complaint Management System form with JPDB integration for data insertion (IML `PUT` command).

## Scope of functionalities
- Capture user inputs (Complaint ID, Name, Email, Description).
- Validate form inputs before submission.
- Construct JSON requests manually as per JPDB standards.
- Send asynchronous `PUT` requests to the JsonPowerDB `api/iml` endpoint.
- Alert user with the response from the server and reset the form.

## Examples of use
1. A customer visits the page and fills out the "Register a New Complaint" form.
2. The user clicks "Submit Complaint".
3. The javascript `validateAndGetFormData()` function ensures all fields are filled.
4. The `createPUTRequest()` function structures the data into a JPDB-compliant JSON object.
5. The `executeCommand()` function fires a POST request to `http://api.login2explore.com:5577/api/iml`.
6. The data is instantly saved in the `COMPLAINT_TABLE` relation inside the `COMPLAINT_DB` database.

## Project status
- **Active:** Form UI and Insert functionality are completed. (Future updates can include Retrieval/GET functions).

## Sources
- [JsonPowerDB Official Documentation](https://login2explore.com/jpdb/docs.html)
