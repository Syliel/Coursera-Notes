Service Oriented Approach
* Most non-trivial web applications use services
* They use services from other applications
	* Credit Card Charge
	* Hotel Reservation systems
* Services publish the "rules" applications must follow to make the use of the
service (API) *Application Program Interface*

Multiple Systems
* Initially - two systems cooperate and split the problem
* As the data/service becomes useful - multiple applications want to use
the information/application

*Producer of API has the data and exports the API and defines the API.
*Consumer is the ones that reads the documentation of the API, writes some
code and then complies with the rules of the API.
*More common to be the consumer...

API Security and Rate Limiting
* The compute resources to run these APIs are not "free"
* The data provided by these APIs is usually valuable
* The data providers might limit the number of requests per day,
  demand an API "key", or even charge for usage
* They might change the rules as thing progress...
