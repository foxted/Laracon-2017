# Taylor Otwell

## Laravel 5.5
- JS Framework presets
- Route::view, return a route without controller, 
- Route::redirect to redirect to another route
- Blade::if directive, custom if statement
- Renderable mailable in the browser
- Renderable exceptions to preview custom error pages
- Responsable, interface on classes to transform to a API Response
- One off notification, without having a user
- Validation Classes for complex validation rules (ex. Github valid repository check)
- Trusted Proxy (Load Balancer / Cloudflare)
- Migrate:fresh, destroy the DB and migrate
- DatabaseTest: DBTransactions, RefreshDatabase trait = make sure DB is up to date and then run tests in transactions
- RoutingTest: withoutExceptionHandling, deactivate the exception reporting
- Dusk now headless
- Package discovery automatically register the ServiceProvider & Facade
- Vendor publish interactive
- Auto registered console commands no need to list artisan commands anymore
- Job chaining: can create a chain of jobs to run one after the other
- Missing models in queue, cancel the job automatically

## Laravel Horizon

Queue package for Laravel: FREE!!!! Available tomorrow.

Dashboard for queues, job monitoring, job tagging, track failed jobs, retry etc…, retry logs :), queue balancing: simple, auto, wait time threshold with notifications, dashboard authentication, easy queue scaling