# week1-personal-info-
#week1@charan#


# ---------------------------------------------------------
# Step 1: Project Setup & Comments
# File: personal_info.py
# Author: Charan
# Description: A program to store personal info and ask for user favorites.
# ---------------------------------------------------------

# ---------------------------------------------------------
# Step 2: Store static information
# ---------------------------------------------------------
# Name is a String (text)
name = "Charan"

# Age is an Integer (whole number)
age = 20

# City is a String
city = "Chennai"

# Hobby is a String
hobby = "Listening to MP3s and playing cricket"

# Step 6b: Calculate age in months
# We multiply the integer 'age' by 12
age_in_months = age * 12

# ---------------------------------------------------------
# Step 3: Get user input (with Validation)
# ---------------------------------------------------------
print("\n--- User Input Section ---")

# Asking for favorite food
fav_food = input("What is your favorite food? ")

# Basic Validation: Check if the input is empty
# strip() removes spaces. If the length is 0, it's empty.
if len(fav_food.strip()) == 0:
    print("⚠️ Warning: You didn't enter a food! Defaulting to 'Unknown'.")
    fav_food = "Unknown"

# Asking for favorite color
fav_color = input("What is your favorite color? ")

if len(fav_color.strip()) == 0:
    print("⚠️ Warning: You didn't enter a color! Defaulting to 'Unknown'.")
    fav_color = "Unknown"

# ---------------------------------------------------------
# Step 4: Display information
# ---------------------------------------------------------
print("\n" + "="*30)
print("      PERSONAL PROFILE      ")
print("="*30)

# We use f-strings (f"...") to insert variables directly into the text.
print(f"👤 Name:          {name}")
print(f"🎂 Age:           {age} years ({age_in_months} months)")
print(f"📍 City:          {city}")
print(f"🏏 Hobby:         {hobby}")
print("-" * 30)
print(f"🍗 Favorite Food: {fav_food}")
print(f"🎨 Favorite Color:{fav_color}")
print("="*30)



# Step 6a: Add a welcome message
print("--------------------------------------------------")
print("👋 Welcome to Charan's Personal Info Program!")
print("--------------------------------------------------")


# ---------------------------------------------------------
# Step 6c: Goodbye message
# ---------------------------------------------------------
print("\n✅ Program finished successfully. Goodbye, Charan!")
