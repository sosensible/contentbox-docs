# Architecture

The following are major system architecture updates we have done in ContentBox 3.

### ColdBox 4 

![](/images/ColdBoxLogo2015_300.png)

We have updated the entire core to leverage ColdBox 4 and modularity.  We have completely re-architected all modules to adhere to ColdBox 4 standards and rely on CommandBox CLI for package management and resolutions.  This update in itself is worth noting as it not only modularized even more ContentBox, but gave it a source code reduction and performance boosts.


### <i class="fa fa-database"></i> Oracle + PostgreSQL Support

<img src="/images/postgresql.png" width="250">
<img src="/images/oracle.gif" width="300">

Oracle and PostgreSQL are now fully supported.


### <i class="fa fa-user-secret"></i> BCrypt Support
The default algorithm for passwords is now based on BCrypt with work factors for better security and entropy. You can read more on bcrypt here: https://en.wikipedia.org/wiki/Bcrypt


### <i class="fa fa-lock"></i> Password Policy
A new password policy is now in place for ContentBox for new and current users, which must be greater than 8 characters with at least one:

* Lower case character
* Upper case character
* Digit
* Special character


### <i class="fa fa-paw"></i> Login Tracker

The ContentBox administrator module now comes with a login tracker which if enabled can track invalid logins and be able to block individual ip addresses from brute-force attempts.  We even track all valid logins into the new ContentBox Security Audit Log.

![](/images/authlogs.png)
![](/images/logintracker.png)

### <i class="fa fa-filter"></i> Rate Limiter

ContentBox now comes with a rate limiter module that can limit count and duration and very configurable.  This can stop denial of service attacks or just penetration hacking attempts.

![](/images/ratelimiter.png)


### <i class="fa fa-gear"></i> Core Settings
Introduction of core and user based system settings. This allows for the distinguishing of what are ContentBox core settings and custom user or module settings when managing them from the geek panel.


### <i class="fa fa-globe"></i> Settings Cluster Storage

![](/images/cluster_settings.png)


You can now decide in which caching engine to store global ContentBox settings. This provides the way to fully scale ContentBox in any cloud provider.


### <i class="fa fa-shield"></i> SSL Support + 
SSL support can now be found everywhere in ContentBox for both the UI and admin modules.  Users can even select specific pages for users to transition into or out of SSL for richer eCommerce or secure experiences.


![](/images/ssl_settings.png)

### <i class="fa fa-language"></i> Internationalization
The majority of all modules have been now translated into English, Spanish, Italian, German and French.  There is still work to do to localize the entire source, but it is coming.

![](/images/i18n.png)

### <i class="fa fa-coffee"></i> ContentBox Express with JRE
Our entire build process has been revamped and now we can produce ContentBox Express editions with included Java runtimes for Linux, Mac OS X and Windows.


### <i class="fa fa-exchange"></i> Automated Asset Pipeline
We have completely re-architected our asset pipeline and ContentBox now comes with an integrated development pipeline for front-end development.  All assets are now tracked via bower and npm.  We have created a developer guide for anybody working with the admin assets and collaborating.


### <i class="fa fa-terminal"></i> CommandBox Integration
All development is now done with CommandBox and all dependencies are tracked via CommandBox.  This provides a smoother update processes for users and also a great workflow for collaboration.

### <i class="fa fa-book"></i> DocBox API Docs
DocBox now generates all API docs with much better documentation and readability.

