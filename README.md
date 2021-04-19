# AWS Lambda Function to convert HTML to PDF

A NodeJS application that will populate JSON data into custom HTML template and then it will generate PDF. The application uses Handlebars which is a templating language,
and Chrome-AWS-Lambda which is a headless chromium which is very similar to Puppetter. The main difference between Puppetter and Chrome-AWS-Lambda is that Puppetter is very large in size so it becomes difficult to use it in Lambda function because of the size constraint so here comes Chrome-AWS-Lambda that offers the same functionalities as Puppetter but it has small size. So it is preferable to use Chrome-AWS-Lambda when you are making a Lambda Function.

This application generates the PDF using HTML template and push it to S3 bucket.

To generate PDF you just have to replace the HTML file with your custom template and replace the JSON data with your desired data.

# Note #
Please install the dependencies by running ## npm install ## do not install the dependencies manually because there are few glitches in the updated versions of Chrome-AWS-Lambda. So it might be possible that your app will crash if you do not follow the instructions properly.
