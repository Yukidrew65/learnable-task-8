# Telephone CLI

A simple interactive Command Line Interface for managing and dialing phone numbers, built with Node.js. 

This project demonstrates the core functionality of maintaining a state (a list of phone numbers) and using the **Observer Pattern** to notify different parts of the system when a specific action (like dialing a number) occurs.

## Prerequisites
- [Node.js](https://nodejs.org/) installed on your machine.

## How to Run
To start the interactive prompt, simply navigate to the project folder in your terminal and run:
```bash
node telephone.js
```

## Available Commands

Once the program is running, you can use the following commands:
- `add <number>`: Add a new phone number to your list.
- `remove <number>`: Remove an existing phone number from your list.
- `dial <number>`: Dial a saved number. This triggers observers that print the number and output a dialing message.
- `list`: Display all saved phone numbers.
- `help`: Show the list of available commands.
- `quit` / `exit`: Exit the CLI.

## Design Patterns Used

- **Observer Pattern**: The `Telephone` class acts as a subject that maintains a list of observers. 
  - `PrintNumberObserver`: Logs the phone number when notified.
  - `NowDiallingObserver`: Logs a custom message ("Now Dialling {number}") when notified.

## Author
Chibueze Yuki Onah
