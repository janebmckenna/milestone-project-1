# Testing 

[Return to README](README.md)

## Contents
[Manual Testing](#manual-testing) \
[User Story Validation](#user-story-validation) \
[Lighthouse Audit](#lighthouse-audit) \
[Validator Testing](#validator-testing)\
[Bugs](#bugs)

## Manual Testing
**Device and Browser Testing**

![Table of Manual Testing](assets/testing/m-testing.png)

**Manual Testing of User Actions**

|**Feature**     |**Action**     |**Expected Bahaviour**     |**Result**     |
|----------------|---------------|---------------------------|---------------|
|NavBar          |Click Logo     |Navigates to homepage      |Pass           |
|NavBar          |Click The Plan |Navigates to The Plan page |Pass           |
|NavBar          |Click Accomodation |Navigates to The Accomodation page      |Pass           |
|NavBar          |Click RSVP     |Navigates to The RSVP page      |Pass           |
|NavBar          |Click Gallery     |Navigates to The Gallery page      |Pass           |
|NavBar          |Hover over The Plan |Text becomes bold |Pass           |
|NavBar          |Hover over Accomodation |Text becomes bold |Pass           |
|NavBar          |Hover over RSVP |Text becomes bold |Pass           |
|NavBar          |Hover over Gallery |Text becomes bold |Pass           |
|Mobile Menu     |Click The Hamburger Icon |Displays Menu items |Pass           |
|Mobile Menu     |Click The Hamburger Icon a 2nd time     |Collapses Menu items      |Pass           |
|Mobile Menu     |Click Home |Navigates to The Home page |Pass           |
|Home Page - Video |Click Play Icon |Video plays on mute  |Pass           |
|Footer          |Click St Macarthans Cathedral |Homepage for St Macarthans Cathedral opens in a new tab |Pass    |
|Footer          |Click Lough Rynn |Homepage for Lough Rynn opens in a new tab |Pass    |
|Footer          |Hover over St Macarthans Cathedral |Text Underlines |Pass    |
|Footer          |Hover over Lough Rynn |Text Underlines |Pass    |
|Plan - Location information |Click St Macarthans Cathedral |Homepage for St Macarthans Cathedral opens in a new tab |Pass    |
|Plan - Location information |Click Lough Rynn |Homepage for Lough Rynn opens in a new tab |Pass    |
|Plan - Location information |Hover over St Macarthans Cathedral |Text Underlines |Pass    |
|Plan - Location information |Hover over Lough Rynn |Text Underlines |Pass    |
|Plan - Location information |Click St Macarthans Cathedral Map|Google Maps location for St Macarthans Cathedral opens in a new tab |Pass    |
|Plan - Location information |Click Lough Rynn Map |Google Maps location for Lough Rynn opens in a new tab |Pass    |
|Accomodation Information   |Click Castle |Homepage for Lough Rynn opens in a new tab |Pass    |
|Accomodation Information   |Click Booking.com |Homepage for booking.com opens in a new tab |Pass    |
|Accomodation Information   |Hover over Castle |Text Underlines |Pass    |
|Accomodation Information   |Hover over Booking.com |Text Underlines |Pass    |
|Accomodation Information   |Click accomodation photo |Booking.com opens in a new tab|Pass    |
|RSVP Form     |Click Send! without providing Name details |Pop up: Please Fill in this Field |Pass    |
|RSVP Form     |Click Send! without providing Email details |Pop up: Please Fill in this Field |Pass    |
|RSVP Form     |Click Send! with non email text in email field|Pop up: Please include an '@' in the email address |Pass    |
|RSVP Form     |Click Send! without toggling a radio button |Pop up: Please select one of these options |Pass    |
|RSVP Form     |Click Send! with Name, Email and RSVP response provided |Thank you page appears |Pass    |


## User Story Validation

|**User Story** |**Outcome** |
|-----|-----|
|_"Website provides them with a means to communicate the details of their vow renewal, capture RSVPs and share content from the first time around."_|The Website delivers all the objectives for the owners of the Site Ashley and Hannah. It contains all pertanient details of thier vow renewal, captures RSVPs and shares photos and video.|
|**First Time User**||
|_Intuitively and easily navigate the site to find content._|answer|
|_Respond with my RSVP._|answer|
|_Be able to establish the particulars and timings of the vow renewal._|answer|
|_Browse the photos of the original Wedding Day._|answer|
|**Returning User**||
|_Confirm timings and arrangements for the day._|answer|
|_Find links to accommodation and venues._|answer|
|_Browse the photos of the original Wedding Day."_|answer|

## Lighthouse Audit

When I initially ran the lighthouse audit I found issues with:
- My images sizes impacting load time, I rectified this by resizing the images and changing the format from .img to .WebP.
- Meta Description in the head for SEO, which I rectified.
- Lack of Title on my iframes, which I rectified. 

Following my work to rectify my final lighthouse audit results are below
![Lighthouse result](assets/testing/lighthouse.png)

## Validator Testing

- HTML

No errors were returned when passing through the W3C validator 
![W3C Validator result](assets/testing/validator-html.png)

- CSS

When I initially passed the site through the Jigsaw Validator it returned a lot of errors originating from bootstrap/java script. I made the decision to test my CSS directly through direct input on the validator. 

Initally one error was found, there was a Parse error on line 275 of my css file. I had missed the second closing curly cracket on my zoom on my hero image. 

After fixing this, no errors were returned when passing through the validator by direct input for a final time.  
![Jigsaw Validator Result](assets/testing/validator-css.png)

**Peer Review**

I reached out to both my cohort and the peer code review channel on slack to gather any feedback and observations on my site and code, I thnak all those who took the time to reivew my work. Additionally I would like to thank my firends and family for taking the time to review the website as a user.

## Bugs

**Resolved Bugs**

|**Bug**|**Resolution**|
|-----|-----|
|Footer not sticking to the bootom of the viewport|Set the min viewport height to 100% and the top margin of the footer to auto |
|Navigation items not displaying as desired|Used bootstrap to impliment a collapsable hamburger icon for the navigation on Mobile devies, Changed the title of Plan page from 'Plan for the Day' to 'The Plan' |
|Form overflowing the window on Mobile|Reduced the collumns for the input window from 40 to 35 |
|Footer breaks on screens below 400px|Introduced a line break|
|Below 350px the Hamburger icon moves below the Ashley and Hannah Logo.| I used a media query to revise the logo and padding for the logo below 350px|

**Unresolved Bugs**




[Return to README](README.md)