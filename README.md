# nifi
Using NiFi to make cron scheduling to predict the forecasting everymonth.

Use NiFi to execute the bash script to activate python environment then execute the python script that wil load the model and preprocess data and make a forecasting. Then it will deactivate python environment. After this Processor It will load the flowfile into RouteOnContent which will capture the ExecuteProcess is success or not then it will alert to the user by email, Another one is UpdateAttribute which is update the filename then Use PutFile which will write the file into directory which will useful for user to see the log of error or success.
