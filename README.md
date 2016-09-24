# Sneha_Assisgnment_QA
Week2

1)	Gmail compose functionality
Acceptance Criteria 

•	To compose a mail, the user should have login credentials to log into the site.
•	The compose email should have designated row for adding recipients, functionalities such as carbon copy(cc), BCC (Blind Carbon copy) should be available, a row for adding subject and body to compose the mail, and a send button.
•	At least one recipient should be added to send the email and should throw an error when no recipient is added and send button is clicked.
•	It should accept any type of email in the recipient.
•	The user should be prompted with a message that the mail was delivered.
•	A popup should be displayed if subject is not provided before clicking on send button.

               BDD Acceptance Criteria
                            Given Gmail login details 
                            When Compose option is selected
                            Then the user verifies for the functionality
                            And presence of elements such as BCC, CC
                            And Send button
               

2)	Transfer amount from one account to other account (dont worry about adding new account)
      Acceptance Criteria 
Pre-Condition: Account is already added

The user should login to the respective bank with valid credentials, and fills the mandatory fields such as selecting the recipient from the list of recipients,  entering valid registered mobile no/email, type of account from which the amount is to be transferred, date to start the transaction clicking on transfer button to initiate the transfer

               BDD Acceptance Criteria
               Given the user logins to the banking portal
                And selects the option transfer to other person
                And user selects the recipient to transfer the amount
                When the amount, date are entered
                And transfer button is clicked
                Then the amount should be successfully available in the receivers account


 
3)	Shopping cart functionality from amazon.com
      Acceptance Criteria
 User selects desired list of products and adds them to shopping cart. Upon checkout this should calculate the price of all the products in the cart including the shipping and taxes applicable.

               BDD Acceptance Criteria
               Given the url of the amazon site
               When user selects the list of products
               And clicks on the Add to cart
               Then all the products should be added to the cart 
                And provides the price of all products including the shipping and taxes applicable




4)	Adding dependent to existing health insurance
     Acceptance Criteria 
User should login to the respective portal, an option for adding dependent is provided with which using dependents are added.

            BDD Acceptance Criteria
             Given User logins to the portal to add dependents
             And an option to add dependent is provided in the home page
            When the user selects the add dependents
            And enters the details of the person to be added
            Then the dependents are added successfully



5)	Remove service from mobile plan
Acceptance Criteria 

User selects the service from the available services and requests for deactivation of that service.
As soon as the deactivate option is chosen that should not be available to the user.

              BDD Acceptance Criteria
Given User access his/her mobile
When Selects the desired service to be deactivated
Then the service should not be available in use to the user

6)	Enrolling student into course
Acceptance Criteria 

To enroll a student into the course, the student should be eligible for the course (check the eligibility) and profile evaluation is done if all the eligibility criteria is met then a successful enrollment is done.

               BDD Acceptance Criteria
               Given The student qualifies for the course to be enrolled for 
               When fills all the required applications
               And Pays the course fee
               Then the student is successfully enrolled into the course

Defects
1)	Facebook and gmail integration is not working
Defect 1: Trying to register with an email that is not registered with the any of the gmail account.
Defect 2: Merging the code impacted the functionality.
Defect 3: Entry of invalid password for logging into the account.

2) Users not able to perform transfer money through chase.com
Defect 1: Server is not up and is giving connection refused.
Defect 2: Selected a recipient who closed their checking/savings account.
Defect 3: Transferring the amount to a person whose account details are not correct (invalid account num, IFSC code)
Defect 4: sending more than the minimum balance is accepted but the transaction is not completed
Defect 5: Failing of DB functionality, in ui added recipients their bank details etc. are not being fetched from DB.

3) Gmail registration (password is visible, email format is not working properly)  (Assuming that it is not designed)
Defect 1: There are no mandatory fields.
Defect 2: No specification for entry of password (length, special characters)
Defect 3: Giving invalid mobile num (more than 10 digits, unregistered num with any of the carrier)
Defect 4: Button Next step is not navigating while clicking.



