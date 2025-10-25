show users' own lisitings in the public section which is explore. so it's make tranparency, consistency and user expericence better
whenI scroll into the lists end it's making unnessary reloadings, I don't even fully scroll to reload, it's just a slight scroll when I come from down to up (heavely noticed only in explore tab)
When I user try delete a listing, in the warning tab it's better if it's "Delete" instead of "Confirm"
Cancle(etc.) mark isn't updating until you reload the my booking section. I mean every time the user come from a booking make the tab refresh or somthing (Don't apply that to the explore tab!!)
The max amounts of the length, width and depth error/warning after enter amount of higher than the recommanded, can't see fully bcz of the layout (my perview on my phone is `max 300...` )
add notification when a user got a booking or message(etc)
add a red dot on booking and messages tabs(etc)
optional : if the notifications are too much, then send a one message called (4+ messges/ Check for books and messages)
And also there a major problem in the address, phone numbers and vehicle regisration numbers. The problem is the user can enter any number or a letter/char for those things
example:  location - 55
          phone number - .
          vehicle regisration - a37dh**
all of them are accepted

recommend : 
  phone numbers:
- phone numbers are often 7-15 numbers included in on all the countries around the world
  
| Country | Example Phone Number|Digits  |
|---------|---------------------|--------|
|   USA   |+1 202-555-0176      |10      |
|   LK    |+94 71 234 5678      |9       |
|   JPN   |+81 3-1234-5678      |9       |
|   BZL   |+55 11 91234-5678    |10-11   |

Location :
- use a Geocoding or Places AUtocomplete API(which is already have)
- then, users type a location name, but can only select from real suggestion.
    example: "Colombo" ✔ ; "asf123"❌ no results;
- When the user submits, send the selected place to geocoding API and comfirm it exists
---
but if you want you can add a Google map or some map and is a map picker. when it's gonna enter a location

  Vehicle registration:
add a feture to confirm it's a real vehicle
- From: collect data of the vehicle (owner name, plate number, make/modle, year, color, location, etc.)
- Verify location: Use autocomple + map picker
- Ask for validate plate number (use regex... WP CAE 1234)
- Upload (optional but recommed) : vehicle photo, registration certi.

  
