# given-when-then
Notes from learning adventures in BDD testing 

End goal of BDD is to create requirements that could be understood by the entire team so as to avoid misunderstandings, helping to ship the feature being developed in the most acceptable way 

BDD attempts to lay out the behavior of the program or feature thru a scenario or set of scenarios that look like:

GIVEN I am an authorized user of the application
WHEN I sign into the application
THEN I should be able to access the application dashboard

with these the qa writes tests to test those scenarios and they should fail first, since it hasn't actually been developed yet.
Then dev creates a feature and tests again, if fail, refactor and repeat tests
Once refactored to acceptance all tests will pass

As defined in the specflow tutorial at https://www.softwaretestinghelp.com/specflow-tutorial/

GIVEN: This is used for describing a set of pre-conditions for the scenario being defined. For instance, in the example, the scenario’s pre-requisite is a logged-in customer. Hence comparing to the Arrange analogy in a unit test, the step implementation will need to ensure that there is a logged in customer.

WHEN: This is used to describe an action or execution step. In the example, it shows that the customer is trying to add a product to his shopping cart. Hence the step implementation for this step will take care of the simulation code to add a product to the cart. This can be compared to the Act step in the Unit tests.

THEN: This is used to describe the Outcome of the scenario and essentially where the validations should be placed in. It can be compared to the Assert step in the Unit testing world. In the example here, the step implementation will assert whether the product got actually added and the quantity is the same as that was chosen by the customer.


Feature Files will group multiple scenarios together according to high level features. 
