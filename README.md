🏨 Hotel Management System

A command-line Hotel Management System built with Python to simulate the core operations of a hotel, including room management, reservations, guest check-in/check-out, booking cancellation, guest search, and booking updates.

This project was built as a practical application of Python fundamentals, with a focus on problem-solving, data structures, functions, file handling, conditional logic, loops, and user interaction.

---

📌 Project Overview

The Hotel Management System is a terminal-based application that allows hotel staff to manage rooms and guest bookings through an interactive menu.

The system provides a simple workflow for:

- 🛏️ Viewing available rooms
- 📋 Viewing room details
- 🧑‍💼 Booking rooms
- ❌ Cancelling bookings
- 🛎️ Checking guests in
- 🚪 Checking guests out
- 🔎 Searching for guests
- ✏️ Updating booking information
- 💾 Storing booking data in a file

The project uses Python dictionaries to represent hotel rooms and a text file to store booking information.

---

✨ Features

🛏️ Room Management

Each room contains detailed information such as:

- Room number
- Room type
- Availability
- Price per night
- Guest capacity
- Room size
- Beds
- Bathroom
- View
- Balcony
- Wi-Fi
- Air conditioning
- TV
- Breakfast
- Mini bar
- Safe
- Living room
- Room service

Different room types are included:

- Single
- Double
- Twin
- Suite
- VIP

---

📋 Available Rooms

Users can view hotel rooms and their complete information before making a reservation.

The system checks the room's availability and displays the relevant room information.

---

🧾 Room Booking

The booking system collects information such as:

- Customer name
- Phone number
- Number of guests
- Selected room
- Check-in date
- Check-out date
- Number of nights
- Total price

The total price is calculated automatically:

Total Price = Room Price × Number of Nights

After a successful booking, the selected room changes from:

available → booked

A booking summary is then displayed using a formatted Rich table.

---

❌ Booking Cancellation

The cancellation system allows a booking to be cancelled after confirmation.

The room's availability is then updated:

booked → available

The system also displays the updated room information.

---

🛎️ Guest Check-in

The system allows a guest to check in after confirming the operation.

The selected room's status is updated to represent that the guest has checked in.

A progress bar is displayed to provide visual feedback during the operation.

---

🚪 Guest Check-out

The check-out system allows a guest to complete their stay.

After confirmation, the room becomes available again:

occupied → available

The updated room information is displayed afterward.

---

🔎 Guest Search

The system can search the booking file using:

- Guest name
- Phone number

This allows hotel staff to locate an existing reservation.

---

✏️ Update Booking

The system provides an interface for modifying booking information, including:

- Guest name
- Phone number
- Check-in date
- Check-out date

---

💾 File Storage

Booking information is stored inside:

booking.txt

The project uses Python's built-in file handling functionality to write and read booking information.

Example structure:

Name | Phone | Check-in | Check-out | Room | Nights | Price

---

🎨 Terminal Interface

The project uses the Rich Python library to make the terminal interface more organized and visually appealing.

It includes:

- Panels
- Tables
- Prompts
- Confirmation dialogs
- Progress bars

Example components used:

Panel()
Table()
Prompt.ask()
IntPrompt.ask()
Confirm.ask()
Progress()

---

🧠 Concepts Practiced

This project was created to apply Python fundamentals in a real-world-style application.

Python Fundamentals

- Variables
- Data types
- Strings
- Integers
- Input/output
- Conditional statements
- "if / elif / else"
- "for" loops
- "while" loops
- Functions
- Dictionaries
- Nested dictionaries
- Dictionary methods
- ".items()"
- ".get()"

File Handling

- "open()"
- Reading files
- Writing files
- "with open(...)"
- ".read()"
- ".readlines()"
- Iterating through file lines
- ".strip()"
- ".split()"

Data Processing

The project also demonstrates how structured information can be stored and processed using dictionaries and text files.

---

🏗️ Application Flow

The main application follows this structure:

                    ┌─────────────────────┐
                    │       START         │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     Main Menu       │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
      Show Rooms          Book Room        Cancel Booking
             │                 │                 │
             │                 ▼                 ▼
             │          Save Booking       Update Room
             │                 │                 │
             └────────────┬────┴─────────────────┘
                          │
                          ▼
                  ┌───────────────┐
                  │ Check-in/out  │
                  └───────┬───────┘
                          │
                          ▼
                  ┌───────────────┐
                  │ Search Guest  │
                  └───────┬───────┘
                          │
                          ▼
                  ┌───────────────┐
                  │Update Booking │
                  └───────┬───────┘
                          │
                          ▼
                  ┌───────────────┐
                  │     Exit      │
                  └───────────────┘

---

🗂️ Project Structure

Hotel-Management-System/
│
├── hotel_management.py
│
├── booking.txt
│
└── README.md

---

🛠️ Technologies Used

Technology| Purpose
🐍 Python| Main programming language
🎨 Rich| Terminal UI and visual formatting
📄 TXT File| Booking data storage
🧠 Dictionaries| Room and booking data
🔁 Loops| Repeated operations and menu logic
⚙️ Functions| Organizing application features

---

🚀 Installation

1. Clone the repository

git clone https://github.com/YOUR-USERNAME/hotel-management-system.git

2. Enter the project directory

cd hotel-management-system

3. Install the required dependency

pip install rich

4. Run the application

python hotel_management.py

---

🖥️ Example Menu

1. Show Available Rooms
2. Book a Room
3. Cancel Booking
4. Check-in Guest
5. Check-out Guest
6. Search For a Guest
7. Update Booking
8. Exit

Enter your choice:

---

📚 What I Learned From This Project

Building this project helped me move beyond isolated Python exercises and start thinking about how multiple programming concepts work together inside one application.

The project gave me practical experience with:

- Designing program flows
- Breaking functionality into functions
- Working with nested dictionaries
- Processing user input
- Managing application state
- Reading and writing files
- Connecting different features together
- Debugging logical problems
- Building a larger Python project from scratch

Most importantly, this project helped me develop a problem-solving mindset instead of only focusing on Python syntax.

---

🔮 Future Improvements

Possible future versions could include:

- [ ] Better error handling
- [ ] Cleaner project architecture
- [ ] Object-Oriented Programming
- [ ] SQLite database integration
- [ ] Multiple booking records
- [ ] Better date validation
- [ ] Improved search system
- [ ] More advanced booking updates
- [ ] Better room-status management
- [ ] Authentication for hotel staff
- [ ] GUI version
- [ ] Web-based version
- [ ] REST API
- [ ] Automated tests

---

🎯 Project Goal

The goal of this project was not simply to create a hotel application.

It was to take the Python concepts I had learned and combine them into a larger, realistic application with interconnected features and persistent data.

This project represents an important step from:

Learning Python Syntax
        ↓
Solving Small Problems
        ↓
Building Functions
        ↓
Working With Data
        ↓
Handling Files
        ↓
Building a Complete Application

---

👨‍💻 Author

Alex

Student & aspiring software developer.

Currently focused on improving my Python programming, problem-solving skills, software development fundamentals, and building real-world projects.

---

⭐ If You Like This Project

Feel free to ⭐ the repository and explore the code.

More projects coming soon.

---

📌 Status

Completed — First Version

The core hotel management workflow has been implemented. Future versions may improve the architecture, data storage, validation, and user experience.


. 