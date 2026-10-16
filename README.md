# Voice-Assistant
# Voice Assistant Using Python

## 📌 Project Overview

The **Voice Assistant Using Python** is a simple voice-controlled application that listens to spoken commands and performs basic tasks such as telling the current time, opening YouTube, opening Google, and exiting the application.

The project uses speech recognition to convert spoken words into text and text-to-speech technology to provide audio responses. It also uses Python's built-in modules to retrieve the current time and open websites through the default web browser.

This project was developed using **Python IDLE** to practise Python programming, speech recognition, voice output, and automation.

## 🎯 Project Objectives

- Develop a basic voice-controlled virtual assistant.
- Convert speech into text using speech recognition.
- Generate spoken responses using text-to-speech.
- Perform tasks based on voice commands.
- Retrieve the current time dynamically.
- Open websites automatically using Python.
- Understand how Python libraries can be combined to build an interactive application.

## ✨ Features

- **Voice Input:** Accepts spoken commands through a microphone.
- **Speech Recognition:** Converts spoken audio into text.
- **Text-to-Speech:** Responds to the user using a computer-generated voice.
- **Time Information:** Announces the current time.
- **Open YouTube:** Opens YouTube in the default web browser.
- **Open Google:** Opens Google in the default web browser.
- **Exit Command:** Stops the assistant when the user says "exit".
- **Time-Based Greeting Function:** Includes a function that can provide a morning, afternoon, or evening greeting.

**Note:** The greeting function is defined in the current code but is not called automatically. The imported `wikipedia` module is also not currently used.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Development Environment:** Python IDLE
- **Libraries:**
  - `pyttsx3` — converts text into spoken audio.
  - `SpeechRecognition` — captures and processes speech recognition requests.
  - `datetime` — retrieves the current date and time.
  - `webbrowser` — opens websites in the default browser.
  - `wikipedia` — imported for potential future Wikipedia-related functionality.

## 📚 Concepts Used

### 1. Speech Recognition

The `speech_recognition` library captures audio through a microphone and uses Google's speech recognition service to convert the audio into text.

### 2. Text-to-Speech

The `pyttsx3` library converts text into spoken responses using the computer's available speech engine.

### 3. Date and Time

The `datetime` module retrieves the current hour and formats the current time for the assistant's response.

### 4. Web Browser Automation

The `webbrowser` module opens websites such as YouTube and Google when the corresponding voice commands are recognized.

### 5. Functions

Functions such as `speak()`, `take_command()`, and `greet_user()` organize the assistant's functionality into reusable blocks.

### 6. Conditional Statements and Loops

Conditional statements identify the recognized command and select the appropriate action. A `while` loop keeps the assistant listening until the user gives the exit command.

## 📂 Project Structure

```text
Voice-Assistant/
│
├── voice_assistant.py
└── README.md
```

## ⚙️ Requirements

- Python 3.x
- Python IDLE or Visual Studio Code
- A working microphone
- Speakers or headphones
- Internet access for Google's speech recognition service

## 📦 Installation

Open the Python IDLE Shell or terminal and install the required libraries:

```bash
python -m pip install pyttsx3 SpeechRecognition wikipedia
```

**Additional note:** Microphone support may require the `PyAudio` dependency. If Python cannot access the microphone, install a compatible PyAudio version for your Python version and operating system.

The `datetime` and `webbrowser` modules are included with Python and do not require separate installation.

## 🚀 How to Run the Project

### Step 1: Create the Python File

Open Python IDLE and create a new file named:

```text
voice_assistant.py
```

Paste your Python code into the file and save it.

### Step 2: Check the Microphone

Make sure your microphone is connected and that Python IDLE has permission to access it.

### Step 3: Run the Application

In Python IDLE, select **Run → Run Module** or press **F5**.

### Step 4: Give Voice Commands

Speak clearly when the application displays the listening message.

Example commands:

- "Time"
- "Open YouTube"
- "Open Google"
- "Exit"

The assistant processes the recognized command and performs the corresponding action.

## 🔄 Application Workflow

1. Initialize the text-to-speech engine.
2. Activate the microphone and listen for spoken input.
3. Send the captured audio to Google's speech recognition service.
4. Convert the recognized speech into lowercase text.
5. Check the command using conditional statements.
6. Announce the current time or open the requested website.
7. Continue listening for more commands.
8. Exit the loop when the user says "exit".

## 💻 Key Functions

### `speak(text)`

Converts the supplied text into spoken audio using the text-to-speech engine.

### `take_command()`

Listens to audio from the microphone, attempts to recognize the spoken words, and returns the command as lowercase text. If recognition fails, it returns an empty string.

### `greet_user()`

Checks the current hour and prepares a suitable morning, afternoon, or evening greeting.

### Main Command Loop

Continuously listens for commands and performs actions based on recognized phrases. The application currently supports checking the time, opening YouTube, opening Google, and exiting.

## 🔐 Limitations and Considerations

- Speech recognition depends on Google's online recognition service.
- A working microphone and suitable audio dependencies are required.
- Recognition accuracy may vary with background noise, pronunciation, and microphone quality.
- The assistant currently supports only a small set of predefined commands.
- The Wikipedia module is imported but not implemented in the current command logic.
- The greeting function is defined but not invoked in the current code.
- The application does not include advanced natural-language understanding or persistent conversation memory.

## 🔮 Future Enhancements

- Automatically greet the user when the assistant starts.
- Add Wikipedia search and spoken summaries.
- Support more websites and desktop applications.
- Add weather information and reminders.
- Improve error handling for microphone and network failures.
- Add more natural voice responses.
- Implement a graphical user interface using Tkinter.
- Add more flexible command matching and confirmation messages.

## 📚 Learning Outcomes

Through this project, I practised:

- Building a basic voice-controlled Python application.
- Using speech recognition to process voice commands.
- Converting text into spoken responses.
- Working with Python libraries and functions.
- Using conditional statements and loops to control program flow.
- Automating browser actions using Python.
- Handling basic speech recognition failures.

