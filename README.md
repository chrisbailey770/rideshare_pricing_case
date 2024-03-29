# Case Study: Pricing a new ride-hailing service
## author: Christopher A. Bailey

This was a fun exercise in using optimization to solve for a 12-month pricing strategy that maximizes profit of a new ridesharing business.

Contained in this repository are:
- **driverAcceptanceData.csv** - data with pay offered to drivers and whether or not they accepted the ride request
- **pricing_strategy_notebook.ipynb** - Python notebook detailing an optimization-based solution for a 12-month pricing strategy

---

*You’re launching a ride-hailing service that matches riders with drivers for trips between Ottawa International Airport and Downtown Ottawa. It’ll be active for only 12 months. You’ve been forced to charge riders $40 for each ride. You can pay drivers what you choose for each individual ride.*

*The supply pool (“drivers”) is very deep. When a ride is requested, a very large pool of drivers see a notification informing them of the request. They can choose whether or not to accept it. Based on a similar ride-hailing service in the same market, you have some data on which ride requests were accepted and which were not. (The PAY column is what drivers were offered and the ACCEPTED column reflects whether any driver accepted the ride request.)*

*The demand pool (“riders”) can be acquired at a cost of $30 per rider at any time during the 12 months. There are 10,000 riders in Ottawa, but you can’t acquire more than 1,000 in a given month. You start with 0 riders. “Acquisition” means that the rider has downloaded the app and may request rides. Requested rides may or may not be accepted by a driver. In the first month that riders are active, they request rides based on a Poisson distribution where lambda = 1. For each subsequent month, riders request rides based on a Poisson distribution where lambda is the number of rides that they found a match for in the previous month. (As an example, a rider that requests 3 rides in month 1 and finds 2 matches has a lambda of 2 going into month 2.) If a rider finds no matches in a month (which may happen either because they request no rides in the first place based on the Poisson distribution or because they request rides and find no matches), they leave the service and never return.*

*Submit a written document that proposes a pricing strategy to maximize the profit of the business over the 12 months.*

---
