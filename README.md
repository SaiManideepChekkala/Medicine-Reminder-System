# 💊 Medicine Reminder System using LPC2148

A simple embedded system that alerts users to take their medicines on time. This project uses the LPC2148 microcontroller along with a 16x2 LCD, 4x4 matrix keypad, real-time clock (RTC), buzzer, and switches. Users can set multiple medicine schedules using the keypad, and the system will trigger alerts when the scheduled time matches the RTC.

---

## 🛠️ Features

- ⏰ Display real-time date and time using RTC on LCD
- ⌨️ Set multiple medicine reminders via 4x4 matrix keypad
- 🔔 Alerts user with buzzer and message on LCD when it’s time
- ✅ Acknowledge alerts using a button press
- ♻️ Automatically resets and runs continuously

---

## 🧰 Components Used

### 🔧 Hardware:
- LPC2148 ARM7 Microcontroller
- 16x2 LCD Display
- 4x4 Matrix Keypad
- On-chip RTC
- Buzzer
- Switches (for input and acknowledgment)
- USB-UART Converter or DB-9 Serial Cable

### 💻 Software:
- Embedded C Programming
- Flash Magic (for flashing hex file)
- Keil µVision IDE

---

## ⚙️ Working Principle

1. **Initialization**: LCD, RTC, keypad, and buzzer are initialized.
2. **Scheduling**: Pressing Switch1 allows users to input multiple medicine times via keypad.
3. **Monitoring**: The system continuously checks the current time against saved schedules.
4. **Alert**: When it’s time, the LCD displays a message, and the buzzer sounds.
5. **Acknowledgment**: User presses Switch2 to stop the alert and resume monitoring.

---

## 🔄 Flowchart

```
Start
  ↓
Initialize peripherals
  ↓
Display RTC time on LCD
  ↓
Wait for user input (Switch1)
  ↓
Save medicine times
  ↓
Check RTC continuously
  ↓
If match found:
    → Display "Take Medicine"
    → Trigger buzzer
    → Wait for Switch2 press
  ↓
Repeat
```

---

## 📦 Project Structure

```
Medicine_Reminder_System/
├── main.c                 # Embedded C source code
├── makefile              # Makefile for compilation (if available)
├── .hex                  # Hex file to flash on LPC2148
├── README.md             # Project documentation
```

---

## 📸 Screenshots

*Add images or circuit diagrams here*

---

## 📤 How to Run

1. Connect components as per the circuit diagram.
2. Load and compile the code using Keil uVision.
3. Flash the hex file to the LPC2148 using Flash Magic.
4. Use Switch1 to set reminder times via the keypad.
5. Wait for alerts at the set times.
6. Press Switch2 to acknowledge and reset the loop.

---

## 📃 License

This project is intended for academic and learning purposes only.

---

## 👨‍💻 Author

**Sai Manideep Chekkala**  
📧 [saimanideep3101@gmail.com](mailto:saimanideep3101@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/sai-manideep-chekkala)  
🔗 [GitHub](https://github.com/SaiManideepChekkala)

