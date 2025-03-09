
<div align="center" style="font-family: 'Lato', sans-serif; color: #333;">
<!--     <img width="80" alt="image" src="https://github.com/user-attachments/assets/aea702a7-0fa7-424a-a536-d3a60af7353d" style="border-radius: 40px; margin-bottom: 20px;"> -->
    <h1 style="font-size: 2.5em; margin: 0;">Hi, I’m Filip! 👋</h1>
    <p style="font-size: 1.2em; margin: 20px 0;">This repository contains a collection of my projects in which the source code is intentionally hidden for security purposes. Enjoy the tour! 🚀</p>
</div>


# Warehouse Management System

![Banner](https://dummyimage.com/1200x300/333/fff&text=Warehouse+Management+System)

Welcome to the **Warehouse Management System** repository! This project is not just another web app—it's a powerful tool crafted to revolutionize warehouse operations. With interactive features and an intuitive interface, it’s built to impress both administrators and clients alike.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
  - [Admin Interface](#admin-interface)
  - [Client Interface](#client-interface)
- [Interactive Demo](#interactive-demo)
  
## Overview
This system simplifies complex warehouse tasks by providing tailored interfaces for different user roles. Whether you need to manage inventory or simply place an order, every function is designed to be efficient, secure, and user-friendly.

## Features

### Admin Interface
- **Product Management:** Add, update, and manage product listings with ease.
- **Company, Department & Category Management:** Organize business partners, departments, and product categories seamlessly.
- **User Management:** Invite and manage user accounts securely.

### Client Interface
- **Product Overview:** Quickly view current products and real-time stock levels.
- **Order Placement:** Place orders for specific dates with a few intuitive clicks.
- **Return Management:** Easily schedule return couriers.
- **Order History:** Access and review all your past orders.

## Interactive Demo
Experience the system in action!  
[👉 Launch the Demo](https://example.com/demo)  


















# Distributed Dictionary Translation System

![Banner](https://dummyimage.com/1200x300/333/fff&text=Distributed+Dictionary+Translation+System)

Welcome to the **Distributed Dictionary Translation System** repository! This project is a sophisticated Java-based application that demonstrates a distributed architecture for real-time word translation. With multiple language servers working together and a user-friendly GUI client, this system is an impressive showcase of network programming, concurrency, and dynamic server management.

**Repository:** [Distributed Dictionary Translation System](https://github.com/malak2284/Dictionary-Translation-System)

## Table of Contents
- [Overview](#overview)
- [Architecture](#architecture)
- [Features](#features)
  - [Main Server](#main-server)
  - [Language Servers](#language-servers)
  - [Dictionary Servers Manager](#dictionary-servers-manager)
  - [Client Handler](#client-handler)
  - [GUI Client](#gui-client)
- [How It Works](#how-it-works)


## Overview
This project implements a distributed dictionary system where a **Main Server** handles client connections and delegates translation requests to dedicated **Language Servers**. Managed centrally by the **Dictionary Servers Manager**, these components work together seamlessly to provide a smooth translation experience via both a command-line interface and an interactive GUI built with Swing.

## Architecture
- **Main Server:**  
  Listens for incoming client connections on port `8000` and dispatches requests using a fixed thread pool.
  
- **Language Servers:**  
  Each server listens on its designated port (e.g., `9001` for English, `9002` for French, `9003` for German) and processes translation requests for a specific language.
  
- **Dictionary Servers Manager:**  
  Initializes default language servers, manages them, and allows for dynamic additions of new language servers.
  
- **Client Handler:**  
  Parses incoming client requests, determines the appropriate language server, and routes the request for translation.
  
- **GUI Client:**  
  Provides an intuitive Swing-based interface for users to input words, select the target language, and view translations in real time.

## Features

### Main Server
- **Concurrent Client Handling:**  
  Efficiently manages multiple client connections using a fixed thread pool.
- **Centralized Routing:**  
  Delegates translation requests to the correct language server based on user input.

### Language Servers
- **Dedicated Language Processing:**  
  Each server is responsible for a specific language, ensuring tailored translation logic.
- **Scalable and Extendable:**  
  Easily add new language servers as needed to support additional languages.

### Dictionary Servers Manager
- **Dynamic Initialization:**  
  Automatically starts default language servers and supports the integration of new ones.
- **Centralized Management:**  
  Maintains and provides information on all active language servers.

### Client Handler
- **Robust Request Parsing:**  
  Validates and processes client input, ensuring correct routing to language servers.
- **Reliable Communication:**  
  Bridges the gap between the client and the appropriate language server efficiently.

### GUI Client
- **User-Friendly Interface:**  
  Built with Swing, offering a responsive and engaging experience.
- **Real-Time Translation:**  
  Enter a word, select a language, and get immediate translation feedback.
- **Interactive and Intuitive:**  
  Designed to impress with its clean layout and ease of use.

## How It Works
1. **Server Initialization:**  
   The Main Server starts on port `8000`, initializing a thread pool and the Dictionary Servers Manager, which in turn launches default Language Servers.
2. **Client Request:**  
   A client (via command line or GUI) sends a translation request formatted as `word,languageCode`.
3. **Request Processing:**  
   The Client Handler parses the request and uses the Dictionary Servers Manager to locate the appropriate Language Server.
4. **Translation:**  
   The Language Server processes the word, applies the translation logic (currently simplified), and returns the translated word.
5. **Response Display:**  
   The client receives the translation and displays it, providing a smooth, interactive experience.







