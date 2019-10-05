This script will give complete details about the sharepoint servers and will start the mandatory services if it is stopped automatically.


-------------------------Ho to deploy or use this script:--------------------------------------------------------------------------------------------

Please follow the below steps to execute the script.

1. Download the Server Reports zip file.
2. Unzip the Server Reports zip file.
3. Copy the Server Reports folder to SharePoint Test server.
4. Open the ServerReports.ps1 file in PowerShell editor. 
5. Look for the below lines and change the parameter value with your actual value.

Input Parameters:
1. $servers = @("Server1","Server2","Server3")  #In line number 92..pass the server name.
2. Configure the "To","CC", "From" and "SMTP" as below:
$To =  "habibur@test.com"
$Cc = "habibur@test.com"
$From = "SharePoint2016@test.com"
$SMTP = "sharepoint.test.com" 

6. save the script.
7. Run the script - if SMPT server is configured in your sharepoint farm, the configured user will get email. 
8. If you find everything is working as expected you can configure this in windows task scheduler.
9. Done!!!
---------------------------Deployment done--------------------------------------------------------------------------------------------------------------