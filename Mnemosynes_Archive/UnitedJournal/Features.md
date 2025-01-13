#projects/united-journal/features

## Miscellaneous 
- **Unique search tags** associated to a database item, which can be back-referenced by users or branches.
	- A lot of companies have very similar names, so it might be nice to be able to prefix accounts with either the name of associated people, the city, or jobs they are up to. 
- **Local Warehouse Database Instance**: The goal is daily customer satisfaction. It would be interesting to look into handling inventory in separate, offline databases hosted at each location. This way even with service outages, we continue to serve the customer.
- **Public Address Product Association Database**: A public database you can enter an address into and see what materials we have provided there in the past. 
	- Warranty, estimated installation date, would be some good info to provide.
	- This could help to drive sales.

## Phone Calls & Numbers
- **Abandoned call analytics**, They already track them in the sense that they are logged. I think it should be handled on a dashboard, where you can take notes on why they called, were they put on hold, happy to hear back, or if they gave an order to key. 
	- It would also be nice to be able to associate those phone numbers to accounts so they can be tracked and linked with other customers.
	- This would be a great addition to the #projects/united-journal/features/crm 
- **Answered call to customer** When a team member answers a call, the phone number is read by the system and pushes a notification to their computer of all associated accounts.
- 

## Orders
- **Order Linking**: Link orders under the same job name, same material list, etc. to help customers keep track of expenses.
- **Automated review** analytics on the order where the items in the cart are compared against past purchases (by the specified customer and in general), and flagged for review if issues are detected. 
	- Examples:
		- 6" White gutter coil and elbows, but with 5" white end-caps. The end-caps would be flagged for review. 
		- White trim coil, black nails. There are so many codes, and accidents do happen.
- **Address linking**: When an address is provided for the order, we can check against our system to see what materials, jobs, etc. have been associated to that address in the past.
- **Project Management**: Link orders to large projects. More info in the [[Project Service]] note. #projects/united-journal/services/project-service
- **Special Order Product Order Dates**: Display information to the team about order days for special order items. *Ex: I think Larry V orders Royal on Tuesdays.*

## Customers
- **Type of Work Note**: When the team hears what kind of work the customer does, we take note of it, and in the future we can send them business. 
	- Auto parsing orders to categorize the team would be something to look into. The definitions would be looser but it is definitely something to look into.


## Branch Feed
More info at [[Feed Service]] note. 
#projects/united-journal/services/feed-service 
- **Branch Event Stream**: Keep current with events (orders, pickups, quotes, new customers, scammers) going on at your branch. 