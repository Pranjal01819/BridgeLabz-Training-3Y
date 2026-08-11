# Assignment 1

## Web Development Fundamentals & Architecture | Practice Codebase Solution

ASSIGNMENT 1
Web Development Fundamentals & Architecture | Practice Codebase Solution
## Question 1: Frontend, Backend, and Full-Stack Development
Web development is divided into three core focus areas based on where code runs and what part of the system it controls:
1. **Frontend Development (Client-Side):** Frontend is everything the user sees, clicks, and interacts with directly in their web browser. It focuses on visual layout, user experience (UX), and design responsiveness using HTML, CSS, and JavaScript (or frameworks like React and Vue).
**Real-World Example:** On Amazon, the search bar, product image gallery, filters, and 'Add to Cart' button are built by frontend developers.
2. **Backend Development (Server-Side):** Backend is the unseen powerhouse that runs on remote servers. It manages server logic, process authentication, interacts with databases, and builds APIs using languages like Node.js, Python, Java, or PHP.
**Real-World Example:** When you click 'Place Order' on Amazon, the backend verifies payment details, updates stock in the database, and sends an order confirmation email.
3. **Full-Stack Development:** Full-stack development combines both frontend and backend skills. A full-stack developer can build an entire web application end-to-end—from the user interface to the database storage.
**Real-World Example:** A developer at a tech startup who creates both the React sign-up form and the Node.js database server logic.

| Aspect | Frontend | Backend | Full-Stack |
|---|---|---|---|
| Where Code Runs | User Browser (Client) | Remote Server / Cloud | Both Client & Server |
| Main Technologies | HTML, CSS, JS, React | Node.js, Python, SQL | HTML, CSS, JS, Node, SQL |
| Primary Goal | User Interface & Experience | Data Processing & Security | Complete End-to-End App |

## Question 2: The Client-Server Model in Web Architecture
The Client-Server model is a simple communication framework where work is divided between two parties: the Client (reque-ster) and the Server (provider).
**Client:** The user's web browser (e.g., Chrome or Safari) that sends requests for web pages or data.
**Server:** A powerful computer listening on the internet that receives requests, processes logic, and returns webpage files or data.
**The Request-Response Cycle:** The client sends an HTTP Request over the network -> The server receives & processes it -> The server sends back an HTTP Response with status code 200 OK.
**Figure: Client-Server Request and Response Architecture Flow**

![Figure: Client-Server Request and Response Architecture Flow](images/figure-1.png)
## Question 3: How a Browser Requests and Displays a Web Page
When you type a URL (e.g., https://example.com) into your browser and press Enter, the following steps occur in milliseconds:
1. **DNS Lookup:** The browser checks its cache or asks a DNS server to convert human-readable domain name (example.com) into a machine IP address (e.g., 93.184.216.34).
2. **TCP/TLS Connection:** The browser connects securely to the server using TCP 3-way handshake and SSL/TLS encryption.
3. **Sending HTTP Request:** The browser requests the page using an HTTP GET command.
4. **Server Processing & Response:** The server fetches index.html and returns an HTTP 200 OK response with the raw code bytes.
5. **Browser Rendering Pipeline:** The browser engine converts raw bytes into visual elements using 4 steps:
- **DOM Construction:** Parses HTML into a tree of document elements.
- **CSSOM Construction:** Parses CSS rules and inline styles into a style tree.
- **Render Tree & Layout:** Combines DOM and CSSOM to calculate element positions and geometry.
- **Painting:** Paints actual pixels, colors, images, and text onto the user's screen.
**Figure: Live Browser Demonstration: Browser Requesting and Rendering index.html via Live Server**

![Figure: Live Browser Demonstration: Browser Requesting and Rendering index.html via Live Server](images/figure-2.png)
## Question 4: Web Development Environment Tools
To build web applications effectively, developers rely on a standard set of core tools:
1. **Code Editor (VS Code):** The primary text editor for writing code. Features syntax highlighting, IntelliSense auto-completion, and extensions.
2. **Web Browser & DevTools (Google Chrome):** Renders web pages and includes built-in Developer Tools to inspect HTML elements, debug CSS styles, and monitor JavaScript console errors.
3. **Version Control (Git & GitHub):** Tracks code history, manages branches, and allows teams to collaborate without losing work.
4. **Runtime & Package Manager (Node.js & npm):** Node.js runs JavaScript on your local machine outside the browser, while npm installs developer packages and libraries.
5. **Terminal / Command Line:** Runs terminal commands, launches local servers, and executes build scripts quickly.
6. **Local Development Server (Live Server):** Spins up a lightweight local server that auto-refreshes your browser immediately whenever you save a file.
## Question 5: What is a Web Server & Common Examples
A Web Server is a combination of hardware and software designed to serve web content over the internet:
**Hardware Web Server:**** A computer connected to the internet that stores website assets (HTML, CSS, images, databases).
**Software Web Server:**** A background application that listens for HTTP requests on port 80/443, validates them, and serves requested files or API data.
Commonly Used Web Servers:
- Nginx: Lightweight, super-fast server widely used for high-traffic websites and reverse proxying.
- Apache HTTP Server: Flexible, open-source traditional web server used globally in shared hosting.
- Apache Tomcat: Specialized Java servlet container for running Java web applications.
- Microsoft IIS: Windows-native web server built specifically for .NET and ASP.NET web applications.
- Node.js (Express): Event-driven server framework commonly used in modern JavaScript applications.
## Question 6: Roles in a Web Project: Frontend, Backend, and DBA
Modern project teams divide responsibilities among specialized roles:
1. **Frontend Developer:** Focuses on user experience (UX) and interface design. Converts mockups into responsive HTML/CSS/JS code and connects UI components to backend APIs.
2. **Backend Developer:** Focuses on server logic and business rules. Builds RESTful APIs, implements security and authentication, and connects the application to databases.
3. **Database Administrator (DBA):** Focuses on data safety and performance. Designs database tables, optimizes queries with indexing, performs regular backups, and manages data security access.
**How They Work Together:** When building a Sign-Up feature, the DBA creates the user table, the Backend Developer builds the registration API endpoint, and the Frontend Developer designs the form UI and sends the user data.
## Question 7: VS Code Setup Guide & Screenshot
Configuring Visual Studio Code for HTML, CSS, and JavaScript development requires a simple setup process:
**Setup Steps:** Download VS Code from code.visualstudio.com -> Install extensions (Live Server, Prettier, ESLint) -> Enable 'Format on Save' in settings.
**Figure: VS Code Development Setup Running HTML, CSS, JavaScript, and Live Server**

![Figure: VS Code Development Setup Running HTML, CSS, JavaScript, and Live Server](images/figure-2.png)
**Screenshot Breakdown:**
- **Left Panel (Explorer):** Shows file structure containing index.html, style.css, script.js, and settings.json.
- **Center Panel (Editor):** Displays HTML5 boilerplate code with linked style.css and script.js files.
- **Right Panel (Live Preview):** Displays real-time preview of the rendered page showing 'Hello World'.
- **Bottom Panel (Terminal):** Shows live-server running on port 5500.
## Question 8: Static vs Dynamic Websites
Websites are categorized into Static or Dynamic based on how content is served to visitors:
**Static Websites:** Deliver pre-built HTML files directly from the server. Every visitor sees identical content. They are fast, cheap, and simple to host.
Example: A personal portfolio site, resume webpage, or restaurant menu.
**Dynamic Websites:** Generate content on-the-fly at runtime using backend code and databases. Content changes dynamically based on user logins, searches, or interactions.
Example: Amazon, Netflix, Twitter/X, or YouTube.
## Question 9: Web Browsers & Rendering Engines
A Web Browser retrieves web resources, while its internal Rendering Engine converts raw code into visual pixels on your screen.
**Five Major Web Browsers & Their Engines:**
1. Google Chrome: Engine: Blink (Chromium project with V8 JavaScript engine).
2. Mozilla Firefox: Engine: Gecko (Independent open-source engine built with Rust).
3. Apple Safari: Engine: WebKit (Apple's native engine optimized for iOS and macOS).
4. Microsoft Edge: Engine: Blink (Built on the Chromium engine).
5. Brave Browser: Engine: Blink (Chromium-based privacy browser).
**How Rendering Engines Differ:**
- Blink focuses on speed, multi-process tab stability, and high performance.
- Gecko focuses on open web standards, parallel rendering, and user privacy.
- WebKit focuses on battery efficiency and smooth GPU integration on Apple hardware.
## Question 10: Basic Web Architecture Flow
Modern web applications follow a clean multi-tier architecture flow:
**Figure: Basic Web Architecture Flow Diagram: Client -> API Gateway -> App Server -> Database**

![Figure: Basic Web Architecture Flow Diagram: Client -> API Gateway -> App Server -> Database](images/figure-3.png)
1. **Client Tier:** The web browser or mobile app that captures user input and sends HTTP requests.
2. **API Gateway:** Validates security tokens, handles rate-limiting, and routes requests to the right server.
3. **Application Server:**** Executes backend code, applies business logic, and queries the database.
4. **Database Tier:** Stores data permanently using relational SQL (PostgreSQL, MySQL) or NoSQL (MongoDB).
