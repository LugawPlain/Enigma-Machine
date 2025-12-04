# Enigma Machine Simulator

A fully functional, web-based simulation of the **Wehrmacht Enigma I** (with Reflector B), widely used during World War II. This project recreates the experience of using the physical machine, complete with rotor mechanics, plugboard connections, and a realistic user interface.

![Enigma Machine UI](https://via.placeholder.com/800x400?text=Enigma+Machine+Simulator+Preview)
*(Note: Replace the placeholder above with an actual screenshot of your application)*

## Features

### ⚙️ Authentic Mechanism
- **Rotors**: Supports 3 rotor slots with selectable rotor types (**I, II, III**).
- **Ring Settings**: Adjustable ring settings (1-26) for each rotor, affecting the turnover notch positions.
- **Stepping Logic**: Implements the correct double-stepping mechanism characteristic of the Enigma machine.
- **Reflector**: Uses **Reflector B** for authentic encryption paths.

### 🔌 Plugboard (Steckerbrett)
- **Custom Connections**: Swap pairs of letters to add an extra layer of security (e.g., `AB CD EF`).
- **Validation**: Real-time validation prevents duplicate connections or self-plugs.

### 🖥️ Interactive Interface
- **Visual Feedback**: Lamps glow realistically when keys are pressed (mouse or keyboard).
- **Textures**: Styled with wood and metal textures to mimic the physical device.
- **Responsive Design**: Works on desktop and mobile devices.

### 📜 Message History & State Management
- **Auto-Save**: Messages are saved to a local history log upon pressing `Enter` or clicking "Save & Clear".
- **State Snapshots**: Each saved message preserves the **exact machine settings** (Rotor positions, Ring settings, Plugboard) used at the *start* of the message.
- **One-Click Restore**: Click any history entry to instantly restore the machine to those settings, allowing you to decrypt the message by simply typing the ciphertext back in.

## How to Use

### 1. Setup
Simply open `index.html` in any modern web browser. No installation or server is required as it runs entirely on client-side JavaScript.

### 2. Configuration
1.  **Select Rotors**: Choose which rotors (I, II, III) go into the Left, Middle, and Right slots.
2.  **Ring Settings**: Set the ring setting (inner ring) for each rotor.
3.  **Initial Position**: Use the ▲ / ▼ buttons to set the starting position of each rotor (e.g., `A A A`).
4.  **Plugboard**: (Optional) Enter letter pairs in the plugboard field (e.g., `AZ BY`) to swap them.

### 3. Encrypting / Decrypting
The Enigma machine is symmetric. To decrypt a message, you must have the **exact same settings** that were used to encrypt it.

1.  **Type your message**: Use your physical keyboard or click the on-screen keys.
2.  **Read the output**: The encrypted (or decrypted) text will appear in the output box.
3.  **Save**: Press `Enter` to save the message and its settings to the history log.

### 4. Using History
- The right-hand panel shows a log of your saved messages.
- **Click** a message to restore the machine to the state it was in *before* that message was typed.
- **Type** the encrypted text again to see the original plaintext.

## License

This project is open source and available for personal and educational use.
