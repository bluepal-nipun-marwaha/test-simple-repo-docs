# Backup of docs/unit_converter_documentation.md
# Created: 2025-12-08T16:19:13.919963
# Commit: 86e081f197ca01b4b7955bd9a5b500df564919b4
# Message: updated and added new file
# Author: bluepal-nipun-marwaha
# Original file: docs/unit_converter_documentation.md
# Backup folder: backup/2025-12-08_16-19-00
# Full documentation backup

---

# Simple Unit Converter

A beginner-friendly Python program that converts common units such as distance, temperature, and weight.  
This project is designed as a small companion utility to a basic calculator.

---

## ✨ Features

The program supports the following conversions:

### **Distance**
- Meters → Kilometers  
- Kilometers → Meters  

### **Temperature**
- Celsius → Fahrenheit  
- Fahrenheit → Celsius  

### **Weight**
- Kilograms → Pounds  
- Pounds → Kilograms  

---

## 📁 Project Structure

```
unit_converter.py   # Main program file
```

---

## ▶️ How to Run

Make sure you have **Python 3** installed.

Run the program with:

```bash
python unit_converter.py
```

You will see a menu like:

```
===== Simple Unit Converter =====
1. Meters → Kilometers
2. Kilometers → Meters
3. Celsius → Fahrenheit
4. Fahrenheit → Celsius
5. Kilograms → Pounds
6. Pounds → Kilograms
```

Enter a number (1–6), then enter the value you want to convert.

---

## 💡 Example

```
Choose an option (1–6): 1  
Enter meters: 500  
500 m = 0.5 km
```

---

## 🛠️ Code Overview

The program contains small helper functions, for example:

```python
def meters_to_km(meters):
    return meters / 1000
```

The `main()` function:
- Shows a menu  
- Accepts the user's choice  
- Performs the selected conversion  
- Displays the result  

---

## 📌 Future Improvements

- Add more unit categories (time, speed, area, volume)  
- Create a GUI version using Tkinter  
- Build a web version with HTML/JavaScript  
- Add error handling for invalid numeric input  

---

## 📄 License

This project is simple educational code — feel free to use or modify it however you like.
