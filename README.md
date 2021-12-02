Drupal 7 custom module

Your task is to create a custom drupal module for Drupal 7 with these features (try to use Drupal API as
much as possible):

1) Name the module “custom_drupal_module”
2) Create custom permissions “show custom page”
3) Create a custom page with URL “custom-page”, set that only users with permission “show custom
page” can see it. On this page set title “Custom page”, below title render 3x the same custom
form (form is described below). Each form should work independently. So on a single page I
will be able to interact with each form separately without reload of the page.

Form features:

Form will have 3 fields:

First field:

Type - radio.
Label for field will be: Node title field type
It will have these 2 values: Select, Textfield
This field is required,

Second field:

When the first field is not set, this field will not be visible. This field will appear and change via AJAX
when the first field is changed.
Label for field will be: Node title
Type - will be variable according value set in first field
This field is required.

In case this field is type of Select, it will have there 3 values:
● First node title
● Second node title
● Third node title

Third field
Type - submit
Value - Submit

This is the submit button. It will submit the form via AJAX. Result message will appear over the button.
(error message when required field is not set, or success message if submit was successful).
When the form  is successfully submit first time, it will CREATE a new Basic page node (machine name
“page”) with language neutral and title of the node will be set from value of Second field. It will then show
message “Node with [NID] was CREATED.”. Each next submit of the form will UPDATE the node it
created before (update the title of the node) and show message “Node with [NID] was UPDATED.”.

Messages should be translatable.
Replace [NID] with real node id;
