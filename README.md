
<div align="center" style="font-family: 'Lato', sans-serif; color: #333;">
<!--     <img width="80" alt="image" src="https://github.com/user-attachments/assets/aea702a7-0fa7-424a-a536-d3a60af7353d" style="border-radius: 40px; margin-bottom: 20px;"> -->
    <h1 style="font-size: 2.5em; margin: 0;">Hi, I’m Filip! 👋</h1>
    <p style="font-size: 1.2em; margin: 20px 0;">This repository showcases a collection of my projects. For security reasons, some projects have their source code intentionally hidden. Enjoy the tour!🚀</p>
</div>


# Warehouse Management System

![Banner]((./moss_beztla.png))

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




# Travel Offers Management System

![Travel Offers](https://dummyimage.com/1200x300/007acc/ffffff&text=Travel+Offers+Management+System)

Welcome to the **Travel Offers Management System** repository! This project is a comprehensive Java-based solution that integrates a MySQL database with a sleek Swing-based GUI to manage and display travel offers. It demonstrates my skills in database management, data parsing, localization, and user interface design—all in one interactive application.

**Repository:** [CODE](https://github.com/malak2284/Travel-Offers-Management-System)




## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [How It Works](#how-it-works)


## Overview
This project reads travel offer data from text files, processes and localizes the information (supporting multiple locales and date formats), and then stores it in a MySQL database. Users can interact with the system via a responsive Swing GUI to view offers, filter by language and date format, and get real-time updates. The solution is designed to be both functional and appealing—ideal for real-world travel agencies or as a proof-of-concept for scalable Java applications.

## Features
- **Database Creation & Management:**  
  Automatically creates a MySQL table to store travel offers and populates it with data read from files.
  
- **Data Parsing & Localization:**  
  Processes raw travel data, localizes country names and travel details based on user-selected locale (e.g., `pl_PL`, `en_GB`), and formats dates according to user preferences.
  
- **Interactive GUI:**  
  A user-friendly Swing interface lets users select language and date format options, then displays travel offers in an interactive table.
  
- **Robust Error Handling:**  
  The system is built to gracefully handle parsing errors and SQL exceptions, ensuring a smooth user experience.

## Architecture
- **Database Class:**  
  Handles MySQL connection, table creation, and data insertion.
  
- **TravelData Class:**  
  Reads and formats travel offer data from external files, supporting dynamic localization using resource bundles.
  
- **Main Class:**  
  Serves as the entry point, demonstrating both console output and the launch of the graphical user interface.
  
- **GUI Implementation:**  
  Utilizes Java Swing components to provide an intuitive interface for viewing and filtering travel offers.

## How It Works
1. **Data Ingestion:**  
   The application reads raw travel offer data from files located in a designated `data` directory.
2. **Data Processing:**  
   Offers are parsed and localized according to the selected language and date format. Country names and places are translated using resource bundles.
3. **Database Population:**  
   A MySQL database is automatically set up with a dedicated table (`offers`), and all parsed travel offers are inserted into it.
4. **Interactive Display:**  
   A Swing GUI allows users to choose language and date format options, and displays the travel offers in a responsive table view.









# Interactive NIO Communication System

![NIO Communication](https://dummyimage.com/1200x300/333/fff&text=Interactive+NIO+Communication+System)

Welcome to the **Interactive NIO Communication System** repository! This project showcases an advanced Java application that combines non-blocking network communication using Java NIO with intuitive Swing-based graphical interfaces. Designed with real-time messaging, topic subscriptions, and dynamic administration in mind, this system demonstrates my expertise in concurrent programming, network protocols, and user interface design.

**Repository:** [CODE](https://github.com/malak2284/Interactive-NIO-Communication-System)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [How It Works](#how-it-works)


## Overview
This project implements a multi-faceted communication system where clients and administrators connect to a central server using non-blocking I/O (Java NIO). The system includes:
- **Client and Admin Applications:**  
  Both provide graphical user interfaces (GUIs) to interact with the server. Clients can manage topics and send messages, while admins can view and control active topics.
- **Server Components:**  
  A robust server (with a dedicated GUI) listens for incoming connections, manages topic-based subscriptions, and forwards messages accordingly. Additionally, a basic echo server is implemented for demonstration purposes.

## Features
- **Non-Blocking Communication:**  
  Utilizes Java NIO with SocketChannels and Selectors to handle multiple concurrent connections efficiently.
- **Graphical User Interfaces:**  
  Developed using Swing, offering separate GUIs for Clients, Admins, and the Server, each tailored for their respective tasks.
- **Topic Management:**  
  Clients can add or remove topics dynamically, while the server supports topic-based subscriptions to filter and forward messages.
- **Interactive and Real-Time:**  
  Immediate feedback and message forwarding provide a responsive, real-time communication experience.
- **Robust Error Handling:**  
  Gracefully handles connection issues, ensuring stable communication between clients and the server.

## Architecture
- **Client & Admin Applications:**  
  Both applications establish non-blocking connections to the server (port 12345) and provide interactive GUIs for sending and receiving messages. The Admin interface also aggregates topics from the Client GUI for enhanced management.
  
- **ServerGUI:**  
  Implements a non-blocking server using a Selector to monitor multiple channels. It manages client subscriptions, logs activity in a Swing-based interface, and forwards messages to subscribers based on topic matching.
  
- **Server (Echo Server):**  
  A simpler server implementation (listening on port 12346) that echoes incoming messages. This component demonstrates fundamental NIO operations and serves as a test bed for network communication.

## How It Works
1. **Connection Establishment:**  
   - Clients and Admins create non-blocking SocketChannels and connect to the ServerGUI.
   - The server registers new client connections using a Selector for efficient I/O operations.

2. **Messaging & Topic Subscription:**  
   - Clients can add topics through their GUI. These topics are displayed dynamically and can be used to filter messages.
   - Admins access a dedicated interface to view and manage these topics.
   - The server monitors incoming messages; if a message includes a subscribed topic, it is forwarded to the relevant clients.

3. **Interactive Communication:**  
   - All components use Swing to offer real-time feedback. Messages and status updates appear instantly on the respective GUIs, ensuring a smooth, interactive experience.



