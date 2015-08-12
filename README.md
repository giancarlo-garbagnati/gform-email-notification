# gform-email-notification
TL;DR - Google Form script that emails the user each time the form is submitted. Only submits fields that were filled in and non-zero.

My friend had a Google form that she was using at work for ordering purposes. The form had a list of items, and for each item the form responder was to enter how many of that item the responder wanted to order. The form was then to trigger an email upon submission of the form with all the inputs by the form responder. However, the current set-up she had was emailing her a list of all the items on the form, regardless of if they were being ordered (n>0) or not (n=0 or blank field).

So I set out to learn enough javascript/google app scripting to be able to do this. I have my solution to the blank emails (which is one of the two files) (with a little help from http://www.labnol.org/internet/google-docs-email-form/20884/ for the initialization step). After I came up with a solution, I got a hold of their current script (which happened to be the same as the solution in http://www.labnol.org/internet/google-docs-email-form/20884/ very very slightly modified), so I modified it further to ignore 0s or blank cases (this is the second file).

To use, open up your google form, then go to Responses -> View Responses. In this spreadsheet, go to Tools -> Script Editor. Copy paste either file's code into the Code.gs field, change the default email to the email you want to use, save, go to Run -> Initialize, and you're good to go.

Once again, have to mention this is my first foray into javascript and google app scripting. My apologies if this isn't the most optimal or elegant solution.
