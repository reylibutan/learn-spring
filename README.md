### Spring Best Practices
* Construction (mandatory) and Setter (optional) injection vs the Field injection 
  * constructor injection adds the ability to use `final` fields which totally makes sense for required dependencies
  * constructor injection forces you to initialize a component *properly* - by forcing you to supply proper constructor args
  * field injection is **unsafe** - initialize improperly and say hello to `NullPointerException`
  * constructor injection allows you to inject dependencies a lot easier during testing
