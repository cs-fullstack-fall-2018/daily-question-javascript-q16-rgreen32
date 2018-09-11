# Daily Question - JavaScript Try/Catch

### Try/Catch/Throw
MSJS practice question 19

The body of the HTML page contains the following script: 
```
    <script>
             var fileInfo = 'Could not process the file';
             var reportInfo = 'The daily report was not generated';
             var invoiceInfo = 'The invoices were not created';
             try {
                      logInfo(fileInfo, reportInfo, invoiceInfo);
             }
             catch (e) {
                      console.log('Could not call the function to log the info!');
             }
             finally {
                      console.log('Executed the finally block');
             }

             function logInfo(info) {
                      var date = new Date();
                      console.log(`INFO: ${info}; LOGGED ON ${date}`);
             }
    </script>
```
* What will be displayed in the console when this page is previewed in the browser?

1) INFO: Could not process the file; LOGGED ON Fri Nov 03 2018 20:19:53 GMT-0400 (Eastern Standard Time)<br/>
Could not call the function to log the info!<br/>
Executed the finally block<br/>

2) Could not call the function to log the info!<br/>
Executed the finally block<br/>

3) INFO: Could not process the file; LOGGED ON Fri Nov 03 2018 20:19:53 GMT-0400 (Eastern Standard Time)<br/>
Executed the finally block<br/>

4) Could not call the function to log the info!<br/>
