## Postmortem: Eccomerce  Comapany
![404 page](img/post404.jpg?raw=true "Title") 
** Issue Summary **
For an e-commerce website, some pages were not responding as they ought to. A very frustrating issue if you plan on ordering the latest Mac book. This affected the users, visitors, and also vendors on the site from `13:00 GMT+1 30 August 2021` and stayed `till 14 GMT+1 31 August 2021`. This problem on the site made some pages inactive by not displaying the content on some products category as a result users and visitors could not add to the cart nor purchase any of those products on the inactive page. On the site of the vendors, their products that were under that category were affected since they could not be seen. This affected and overall 78% of those using the site. This problem was a result of a wrong link. The page was referring to another link that was recently deleted and as a result, the affected pages displayed a 404 error.
###  Timeline
- 13:00 GMT + 1 30 August 2021: Issue detected by a worker of the company, not in the web development sector.
- 13:15 GMT+1 30 August 2021 issue reported to someone present in the software sector
- 13:30 GMT+1 30 August 2021: The junior developer checks the problem to confirm the claim.
- 14:30 GMT+1 30 August 2021: Junior developer looks for other affected pages and suspected a malicious attack on the software as a result search for a sign of false entry. 
- 16:28 GMT+1 30 August 2021 The incident is then escalated to the senior developer, who is notified via message
- 12:50 GMT+1 31 August 2021 Senior developer notices the fault of the wrong link on the WordPress dashboard of the site.
- 13:30 GMT+1 31 August 2021 the wrong links are replaced with the right one
- 14:00 GMT+1 31 August 2021 the site is tested and it shows that everything is working fine.

![Search](img/search.jpg?raw=true "Title")
### Root Causse and Resolution
The website had some repeated pages and in order to make the backend and the website less complicated, these duplicated and repeated pages had to be deleted permanently. While deleting different products and pages the deleted link was still used to refer to key pages on the site as a result those pages returned a 404 error.
The issue was fixed by going back to the WordPress dashboard, reviewing the parent pages of the problematic page, and checking the link which is contained, once the wrong link was discovered, the correct link was inserted instead of the wrong one.
## Corrective and Preventative Measures.
- In order to avoid this problem, the following can be done:
- Organize the structure of the site before creating pages.
- When a page is deleted, the parent page should be updated by removing the broken link.
