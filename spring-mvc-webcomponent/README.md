# Sakai Widget Webcomponent Tool
This example shows the basic structure of a clientside single page webapp sakai tool that can create, read, update and delete (CRUD).
It should serve as a guide to demonstrate features and recommended practices. The tool will be updated with more
features in the future and I will add more documentation to the tool as those features are added.
## Application Structure
* Persistence
  * Uses JPA annotations to model POJO
  * Spring Data Repository style for managing the POJO's persistence
  * Spring Transaction Management
  * Hibernate ORM
* Business Logic
  * Spring Framework for Dependency Injection
  * The logic of the app
  * Unit tests that test the application logic
  * Integrates with many other services and features in Sakai
* Serverside
  * Spring MVC - uses springs REST Controller to handle requests to and from the client
  * Thymeleaf - templating framework for creating the initial single page webapp
* Clientside
  * lit-element - for creating the custom sakai-widget element
  * lit-html - templating engine used on the client side
## How to use
This assumes you have a working Sakai system for *personal* use.
1. git clone
1. maven clean install
1. cd spring-mvc-webcomponent
1. maven sakai:deploy-exploded
1. start tomcat
1. create a site in sakai
1. goto "Site Info" -> "Manage Tools" and add the Widget Tool
1. click on the widget tool that has been added to the tool menu

## TODO
My goal here is to advance this tool and create / show good patterns that developers can use in their own tools.
In the future will see more additions that show case features in sakai, here is a small list:
- [ ] Permissions
- [ ] Skin (morpheus)
- [ ] Accessibility (a11y)
- [ ] Events
- [ ] Rich Text Editor
- [ ] Rich UI Elements
- [ ] Import Data to other Sites
- [ ] Security
- [ ] Resources
- [ ] Entity Broker
- [ ] Search
- [ ] Linking (EL Finder)
- [ ] Notifications
- [ ] Caching (to improve performance)
