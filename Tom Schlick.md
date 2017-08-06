# Tom Schlick - Built multi-tenant apps RunMyBusiness

### DB strategies
#### Single DB
All tenants in DB, tenant_id on each table to segment data

- Scoping queries
- Global query scope

#### Multiple DB

Separate DB per tenant + shared database with a “router” 

2 connections in Laravel: shared + tenant. Service Provider to load subdomain and connect to the DB, Tenant model to handle change of DB

Billing data on the shared DB


Pros:
Single point where data is segmented, Easy to test. Reduced points of failure. Less chance of data being exposed.
Third party packages of the shelf, no modifications
Long term scalability
Portability: easy to export & backup
Enterprise transition to on-premise version
Clusters

Cons: 
Complex migrations

### How to choose?

- Need to display multiple tenants on the same page = single
- Need to segment, export or privately host data = multi
- Third party packages = multi preferred
- Highly sensitive data = multi

Separate the storage for each tenant as well (easy to export/backup). For search, indexes for each tenant. Same for cache. Override configuration on runtime.

External services (Mailgun, any API): provide tenant ID

### Domain strategies
- Work on both single & multi
- Branding
- Multiple subdomains
- DNS to choose which server to handle which customer


### Packages

HipsterJazzbo/Landlord
Tomschlick/TownHouse