# telnyx_tests_cypress
Test cases for https://telnyx.com/
Node js v18.7.0 or higher should be preinstalled
Framework: cypress version 10.8.0 or higher
Start tests use commandline: npx cypress open
Then follow the instructions posted at https://docs.cypress.io/guides/getting-started/opening-the-app from the section "The Launchpad"
After starting a new browser session, click on "main.spec.cy.js"

Test scenario ID: Functionality and display of page elements-1
Test case ID: Functionality and display of page elements-1A
Test case description: Checking basic functionality and display of page elements

ID:01
Title: Сheck header for sections availability
Steps:
1. goto https://telnyx.com/
2. Check main page header for 'Solutions', 'Network', 'Resources', 'Company', 'Pricing' availability
Expected result: 'Solutions', 'Network', 'Resources', 'Company', 'Pricing' are available.   

ID:02
Title: Check header to contain some text
Steps:
1. goto https://telnyx.com/
2. Check header to contain 'Talk to an expert'
Expected result: Header contain 'Talk to an expert'.   

ID:03
Title: Check title to have some text
Steps:
1.goto https://telnyx.com/
2. Check title to have 'Telnyx | Communication APIs for Seamless Connectivity '
Expected result: Title contain 'Telnyx | Communication APIs for Seamless Connectivity '.   		

ID:04
Title: Should add value to email field
Steps:
1. goto https://telnyx.com/				 
2. Type in email field 'test123@gmail.com'
Expected result: 'test123@gmail.com' should appear in email field.   					 

ID:05
Title: Should redirect to sign-up page from empty email field
Steps:
1. goto https://telnyx.com/				 
2. Click on email field 
3. Press 'Enter' button on keyboard
4. Check url to include:'/sign-up' 
Expected result: https://telnyx.com/sign-up page was displayed. 

ID:06
Title: Should redirect to sign-up page from filled email field
Steps:
1. goto https://telnyx.com/				 
2. Type in email field 'test123@gmail.com' 
3. Press 'Enter' button on keyboard
4. Check email field on sign-up page to contain previously enterd email
5. Check url to include:'/sign-up' 
Expected result: https://telnyx.com/sign-up page was displayed, 'test123@gmail.com' should appear in email field. 

ID:07
Title: Should redirect to sign-up page by header link
Steps:
1. goto https://telnyx.com/				 
2. Click on 'Sign-up' button in header 
3. Check url to include:'/sign-up'
Expected result: https://telnyx.com/sign-up page was displayed.

ID:08
Title: Should redirect to sign-up page by footer link
Steps:
1. goto https://telnyx.com/				 
2. Click on 'Sign-up' button in footer 
3. Check url to include:'/sign-up'
Expected result: https://telnyx.com/sign-up page was displayed.

ID:09
Title: Should redirect to login page by header link
Steps:
1. goto https://telnyx.com/				 
2. Click on  'Login' button in header 
3. Check url to include:'/login/sign-in'
Expected result: https://portal.telnyx.com/#/login/sign-in page was displayed.

ID:10
Title: Sign-up with not valid credentials, some error message should be visible
Steps:
1. goto https://telnyx.com/				 
2. Click on 'Sign-up' button in header  
3. Type in email field some fake email
4. Type in name field some fake name
5. Type in password field some fake password
6. Click on checkbox:'I agree to the Terms and Conditions and Telnyx's Privacy Policy'
7. Click on 'Submit' button
Expected result: some error message was displayed.