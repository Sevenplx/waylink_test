# Executive Summary – App Testing Feedback Day 02(10/25/25)

During testing, I identified several usability issues, potential bugs, and areas for improvement. These findings focus on enhancing user experience, navigation flow, and form handling efficiency.

## Key Findings

- **Explore Section – User Listings:** Show users’ own listings in the public Explore section to improve transparency, consistency, and user experience.  
- **List Reload Bug:** Slight upward scrolls at the top of the list trigger unnecessary reloads (noticed mainly in the Explore tab).  
- **Delete Confirmation:** When a user tries to delete a listing, change the warning button from “Confirm” to “Delete” for clarity.  
- **Booking Tab Refresh:** Cancel/other status marks don’t update until reloading the My Booking section. Ensure the tab refreshes when users return (but do not apply this to Explore).  
- **Length, Width, Depth Warnings:** Error messages for values exceeding the maximum are cut off in the layout (e.g., “max 300…” not fully visible).  
- **Notifications:** Add notifications when a user receives a booking or message.  
- **Red Dot Indicators:** Add a red dot on Booking and Messages tabs.  
- **Optional Notification Summary:** If notifications are numerous, send a single message like “4+ messages / Check bookings and messages.”  
- **Data Validation – Address, Phone, Vehicle Registration:** Currently, users can enter invalid numbers or characters:  
  - Example: location `55`, phone `.` , vehicle registration `a37dh**` — all are accepted.  
- **Phone Numbers:** Validate numbers globally (7–15 digits). Examples:  

| Country | Example Phone Number | Digits |
|---------|-------------------|--------|
| USA     | +1 202-555-0176    | 10     |
| LK      | +94 71 234 5678    | 9      |
| JPN     | +81 3-1234-5678    | 9      |
| BZL     | +55 11 91234-5678  | 10–11  |

- **Location Validation:**  
  - Use a Geocoding or Places Autocomplete API.  
  - Users type a location name but can only select from real suggestions. Example: "Colombo" ✔ ; "asf123" ❌.  
  - On submit, confirm the location exists via the API.  
  - Optional: Add a map picker to select the location visually.  
- **Vehicle Registration Validation:**  
  - Collect vehicle data: owner name, plate number, make/model, year, color, location, etc.  
  - Verify location via autocomplete and map picker.  
  - Validate plate number using regex (e.g., WP CAE 1234).  
  - Optional: Upload vehicle photo and registration certificate.  

---

# Longer and More Detailed Test Report Feedback

Let's go through everything I noticed while testing the app — including potential bugs and areas of confusion:

1. Show users’ own listings in the public Explore section for transparency and consistency.  
2. Slight upward scrolls at the top of the list trigger unnecessary reloads (noticed mainly in the Explore tab).  
3. When deleting a listing, the confirmation button should read “Delete” instead of “Confirm.”  
4. In My Booking, cancel/other status marks do not update automatically. Refresh the tab when users return (don’t apply to Explore).  
5. Error messages for exceeding length, width, and depth are truncated in the layout (e.g., “max 300…”).  
6. Add notifications for new bookings or messages.  
7. Display a red dot on Booking and Messages tabs.  
8. Optional: If notifications are numerous, send a summary message (e.g., “4+ messages / Check bookings and messages”).  
9. Data validation issues: addresses, phone numbers, and vehicle registration numbers currently accept invalid inputs:  
   - Location: `55`  
   - Phone number: `.`  
   - Vehicle registration: `a37dh**`  
10. **Phone Numbers:** Validate 7–15 digits globally. Examples:  

| Country | Example Phone Number | Digits |
|---------|-------------------|--------|
| USA     | +1 202-555-0176    | 10     |
| LK      | +94 71 234 5678    | 9      |
| JPN     | +81 3-1234-5678    | 9      |
| BZL     | +55 11 91234-5678  | 10–11  |

11. **Location Validation:**  
    - Use a Geocoding or Places Autocomplete API.  
    - Users can only select from valid suggestions (e.g., "Colombo" ✔ ; "asf123" ❌).  
    - Confirm the selected place exists via API.  
    - Optional: Map picker for location selection.  
12. **Vehicle Registration Validation:**  
    - Collect full vehicle data (owner, plate, make/model, year, color, location).  
    - Verify location with autocomplete + map picker.  
    - Validate plate number format using regex (e.g., WP CAE 1234).  
    - Optional: Upload vehicle photo and registration certificate.  

---

**Note:** These are just some observations and ideas to make the app even better. Overall, the app is looking solid, so think of this as friendly feedback rather than anything urgent.
