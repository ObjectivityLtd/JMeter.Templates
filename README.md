# JMeter.Templates introduction
These templates were created for an earlier JMeter version but work just fine with the latest one (currently 5.4.3) as well.<br>
Make sure to copy template files (.jmx) as well as templates.xml file to bin\templates location and restart JMeter.

# OBJ JDBC Load Test
Template showing how to Load Test an SQL query on Database.

## JMeter Configuration
* In **User Defined Variables** and **JDBC Connection Configuration** configure the Server's: 
	* URL or IP, 
	* port, 
	* number of threads and iterations,
	* username and password 

* Modify the SQL queries in **Common DB queries** to match your query.

# OBJ Structure and record a throughput based web test plan
Template showing how to structure a thoroughput web test plan and record your application's requests.

## JMeter Configuration
* Add each of your business transactions under a transaction controller
* Place the transaction controllers inside **Functionalities** component
* Create a new **Thread Group** component for each of your business transactions
* Specify a required thoroughput for you business transaction
* Use module controller to attach your business transaction in the **Thread Group** component

## JMeter Record Configuration
* In **HTTP(S) Test Script Recorder** component JMeter port is set to 8888 - you may need to change this.

## Browser Configuration
* Configure your browser so that it uses the JMeter proxy.

# OBJ Structure and record a web test plan
Template showing how to structure a web test plan and record your application's requests

## JMeter Configuration
* Add each of your business transactions under a transaction controller
* Place the transaction controllers inside **Functionalities** component
* Use module controllers to attach your business transactions in the **Thread Group** element

## JMeter Record Configuration
* In **HTTP(S) Test Script Recorder** component JMeter port is set to 8888 - you may need to change this.

## Browser Configuration
* Configure your browser so that it uses the JMeter proxy.
