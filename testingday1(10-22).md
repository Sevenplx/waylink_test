# Executive Summary – App Testing Feedback

During testing, I identified several usability issues, potential bugs, and areas for improvement. These findings focus on enhancing user experience, navigation flow, and form handling efficiency.

## Key Findings

- **Navigation:** Using the phone’s back button exits the entire app instead of going to the previous screen.  
- **Create Listing Button:** Should be a sticky button for easier access.  
- **Phone Number Field:** Auto-detect user location for default country code and make it a searchable dropdown.  
- **Flight Search:** Allow searching by country and airport name interchangeably.  
- **Currency Selection:** Replace dropdown with a searchable input.  
- **Location Suggestions:** Suggest previously used locations when adding new listings.  
- **Road Listings:** Add an “Other” option for vehicles and suggest country-specific ones.  
- **Welcome Screen:** Improve design and image loading speed (use WebP or similar).  
- **Loading Screen:** Make the loading screen simpler, so it will load faster to the app (some users are in a hurry).  
- **Weight Units:** Add more units and allow decimal values.  
- **Terminology:** Consider using “Length” instead of “Depth.”  
- **Data Persistence:** Add caching/draft saving to prevent data loss on accidental exits.  
- **Listing Flow:** Prevent exiting mid-listing without saving or discarding.  
- **Image Upload:** Prevent duplicate image uploads.  
- **Flight Number Field:** Validate format (e.g., [1–2 letters][1–4 numbers][optional letter]).  
- **T&C Confirmation:** Previously repeated prompts — may now be fixed.  
- **Listing Interaction:** Make the entire listing card clickable, not just the “Deliver/Book” button.  

## Summary
Overall, the app shows good functionality but could benefit from UX refinements, validation improvements, and smoother navigation. These suggestions aim to enhance user satisfaction and reduce friction during core interactions.

---

# Longer and More Detailed Test Report Feedback

Let's go through everything I noticed while testing the app — including some bugs (possibly) and areas of confusion I experienced while using it.

1. When I tried to go back using the navigation buttons on my phone, it exited the entire app. I think this is a drawback because it resets the app, and I have to redo everything I was doing at that time.  
2. The “Create Listing” button is usually located at the bottom of the form. Personally, I’d prefer if it were positioned as a sticky button.  
3. On the form where the contact number is entered, make it detect the user’s location and automatically set the country code by default. Also, make the country code field a searchable dropdown so users can easily find their code without typing it manually.  
4. When searching for flights, even if I search for a country instead of a specific airport, it should still return relevant results (airport name and country name).  
5. For currency selection, add a search bar instead of only a dropdown — it’s easier to use.  
6. When a user creates a new listing, fetch and suggest locations that the user has used previously.  
7. When creating a road listing, add an “Other” option so users can enter details manually. Also, suggest available vehicles for that specific country.  
8. The welcome screen looks a bit unprofessional. If you plan to keep it, improve the design and image quality. Also, the images take too long to load — consider using WebP or another optimized format.  
9. Make the loading screen simpler, so it will load faster to the app (some users are in a hurry).  
10. Add more weight units (e.g., grams) or allow decimal values (e.g., 0.000).  
11. I’m not completely sure about this, but consider using “Length” instead of “Depth” for better user understanding.  
12. Add caching or local saving, so if a user accidentally closes the app while making a listing or sending a message, their entered data isn’t lost.  
13. Prevent users from leaving the listing creation process without either completing or discarding it — maybe by allowing them to save a draft.  
14. When creating a listing, block the ability to add the same image multiple times.  
15. Implement a real flight number validation method (usually: [1–2 letters][1–4 numbers][optional letter]).  
16. When I first used the app, it repeatedly asked me to confirm the Terms & Conditions (I think this issue might be fixed now).  
17. Clicking only on the “Deliver/Book” button might confuse new users. Allow clicking anywhere on the container to view the listing details. (Keep the button, but make the whole area clickable.)  

---

## Questions for Clarification

To make my next test report more accurate and effective:

- Could you provide me with the MVP version of this app?  
- What is the main purpose of this app?  
- Who is the target audience of this app?  
- Could you share some examples of similar apps?  

---

Please don’t think I’m only focusing on negatives — I’m just highlighting things that could help improve the app.  
I hope this feedback helps a lot, and you can look forward to more detailed test reports from me in the future.
