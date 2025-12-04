# 🎢 Six Flags Qiddiya City Event Booking System

A web-based **event booking system** inspired by the Six Flags َQiddiya City theme park experience.  
The system allows **customers** to browse events and book tickets, and provides an **admin dashboard** to manage events and view bookings.

---

## Tech Stack

- **Frontend:** HTML, CSS (`User-style.css`, `Admin-style.css`)
- **Backend:** PHP (procedural)
- **Database:** (`event_booking` database)
- **Sessions:** PHP `$_SESSION` for authentication and cart management

---

## Project Structure (Main Files)

### User Side

- `main.php` – Landing page (Six Flags style) with hero section, attractions, and a **“Start Booking”** button.
- `index.php` – User **Login** page.
- `register.php` – User **Registration** page.
- `home.php` – Shows all available events in a responsive grid with **“Book Now”** buttons.
- `event.php` – Event details page (date, time, location, description, price, remaining tickets) + **Add to Cart**.
- `cart.php` – Shopping cart + **Reserve Tickets** + user booking history.
- `logout.php` – Ends the session and logs the user out.
- `config.php` – Database connection shared by all pages.
- `User-style.css` – Styling for all user-facing pages.

### Admin Side

- `admin.php` – Admin **Login** page.
- `admin_sidebar.php` – Reusable sidebar for the admin dashboard.
- `manageEvents.php` – List and manage all events (view, edit, delete).
- `addEvent.php` – Add new events.
- `editEvent.php` – Edit existing events.
- `deleteEvent.php` – Securely delete events (only if they have no bookings).
- `viewEvent.php` – View full event details (admin view).
- `viewBookings.php` – View all bookings (reports for admin).
- - `config.php` – Database connection shared by all pages.
- `event_booking.sql` – Database 
- `Admin-style.css` – Styling for the admin dashboard (sidebar, tables, cards, buttons).


---

## Authentication & Verification

### User Registration (`register.php`)

- Validates that all fields are filled.
- Checks that **password** and **confirm password** match.
- Verifies **email uniqueness**:

  ```php
  SELECT * FROM users WHERE email = '$email'
---
  ## UI previews 

Below are some UI previews from the user and admin interfaces of the project:

###  Home Page (User)


### Event Details

###  Cart & Booking

###  Login / Register

###  Admin Dashboard

###  Manage Events (Admin)

---


