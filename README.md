# Gym-Booker-project
Automate your gym reservations and never miss a workout slot again!   Post-COVID, gyms like **McGill** introduced online time-slot reservations for safety.   **Gym-Booker** is a Python bot powered by Selenium that automatically books your preferred workout session for you.
# 🏋️‍♂️ Gym-Booker

Automate your gym reservations and never miss a workout slot again!  
Post-COVID, gyms like **McGill** introduced online time-slot reservations for safety.  
**Gym-Booker** is a Python bot powered by Selenium that automatically books your preferred workout session for you.

---

## 🔎 Overview
Gym-Booker takes care of the entire booking flow:
- Logs into your gym account using saved credentials
- Navigates through the reservation system
- Books your chosen slot (and adapts the ID for future days)
- Sends a confirmation email to your student Outlook account  

---

## ✨ Features
- **Automated Navigation** – Reaches the booking section without manual clicks  
- **User Authentication** – Securely logs in with your credentials  
- **Dynamic Slot Booking** – Picks the right session daily by adjusting booking IDs  
- **Email Confirmation** – Get booking details delivered straight to your inbox  
- **Daily Automation** – Schedule with `crontab` (Linux/macOS) or Task Scheduler (Windows)  

---

## ⚙️ Setup & Usage

### 📌 Prerequisites
- Python 3.x installed  
- [Selenium](https://pypi.org/project/selenium/) → `pip install selenium`  
- Google Chrome + [ChromeDriver](https://chromedriver.chromium.org/) (matching versions)  

### 🚀 Steps
1. **Add Your Credentials**  
   - Open `gym_booker.py`  
   - Enter your **username** and **password** at the top  

2. **Choose Your Workout Slot**  
   - Go to the gym booking site → Inspect your preferred workout → Copy the slot ID  
   - Paste the ID into `workout.txt`  
   - The bot auto-adjusts this ID for future days  

3. **Run the Bot**  
   ```bash
   python gym_booker.py
