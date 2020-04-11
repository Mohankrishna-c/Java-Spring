# Java-Spring
Spring, Hibernate, Springboot projects
# a small Spring MVC Cusotomer form validation using Spring MVC and Hibernate Validator.
# A small customer form with 5 fields are used. First name, lastname(which is mandatory), free passes, Postal address.
# Here is the criteria, free passes fields accepts only numbers from 0-10 and not strings.
# I have handled this using 
  @NotNull( message = "is required")
	@Min(value = 0, message = "value should be greater than or equal to 0")
	@Max(value =10, message = "value should be less than or equal to 10")
  these are from Hibernate jars(javax.validation.constraints.*)
  --------------------------------------------------------------------------------------------------------
  # lastname is handled through 
  @NotNull( message = "is required")
	@Size(min=1, message = "is required") which is similar to free pass's field.
  ----------------------------------------------------------------------------------------------------------
  If all the criteria's are satisfied, it will take to confirmation page which lists all the details user have entered.
