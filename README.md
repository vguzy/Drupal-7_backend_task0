 # Drupal 7 custom module
 
 Your task is to create a custom drupal  module for  Drupal 7  with these features (try to use Drupal API  as 
 much as possible): 
 
 1)   Name the module “  custom_drupal_module  ” 
 2)   Create custom permissions “  show custom page  ” 
 3)   Create a custom page with URL “  custom-page  ”, set that only users with permission “  show custom 
 page  ” can see it. On this page set title “  Custom page  ”, below title  render custom form  (form is 
 described below). 
 
 Form features: 
 
 Form will have 3 fields: 
 
 First field: 
 
 Type -  radio.   
 Label for field will be:  Node type 
 It will have these 2 values:  article,    page 
 This field is  required,   
 
 Second field: 
 
 Label for field will be:  Node title 
 Type - Textfield 
 This field is  required.   
 
 Third field 
 Type -  submit 
 Value -  Submit 
 This is the submit button. It will submit the form  via AJAX.   Result message will appear over the button. 
 (error message when required field is not set, or success message if submit was successful). 
 
 When the form  is successfully submit it will CREATE a new node. Type of the node will be taken from the 
 first field  (“  article  ” or “  page  ”), language will be neutral  and title  of the node will be set from the value of 
 Second field.   It will then show translatable success message “Node with [NID] was CREATED.”. 
 Replace [NID] with real node id;
