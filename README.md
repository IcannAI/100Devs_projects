# 100Devs_projects Software Engineering Bootcamp

## MVP Development
### Summary
This session focuses on the final push to complete the Minimum Viable Product (MVP) for the 100-hour capstone project, a critical portfolio piece for the job hunt. The instructor emphasizes prioritizing core functionality over complex design by using tools like Tailwind CSS and DaisyUI to speed up development. The session also transitions into "Hunttober," outlining the upcoming curriculum (React, Data Structures, Algorithms) and stressing the importance of community networking, consistent public building, and leveraging the support of the "100Devs" community to secure employment.

Note 1: MVP Development & Strategy
This section outlines the technical approach to finishing the capstone project efficiently.

### Workflow
Scope the MVP: Distill your 100-hour project idea into its simplest version that still conveys the core functionality.

Extend Existing Code: Use the "Binary Upload Boom" project as a foundation and modify it to fit your specific idea (e.g., changing it from social media to a recipe app).

Prioritize Function over Design: Do not stress about writing custom CSS or perfect copy initially. Focus on getting the core logic working first.

Use Templates: Look at design templates (e.g., ThemeForest, Dribbble) for inspiration on layout so you don't waste cycles designing from scratch.

Submission: The MVP is due by the start of the next class (Tuesday), giving a 24-hour buffer to finalize.

### Tools
Tailwind CSS & DaisyUI: Recommended for rapid styling. Tailwind provides utility classes, while DaisyUI offers free, open-source pre-made components (like navbars and footers) that speed up development.

Bootstrap: An alternative to Tailwind for quickly making a site look decent without custom styling.

Heroku: Currently used for hosting, though the instructor notes a need to switch providers soon due to pricing changes.

Repl.it / CodePen: Useful for quickly testing code snippets or components.

EJS: The templating engine used in the current tech stack, which works well with Tailwind/Bootstrap classes.

### Guidelines
"Quick and Dirty": The MVP should be a rough draft. Refinement and "making it beautiful" come during the remaining 100 hours of development.

Don't Build Alone: Utilize community platforms like Remo (tables for co-working) and Discord (voice channels) to work alongside others and avoid isolation.

GitHub Repositories: Submitting a GitHub link is sufficient for the MVP; live hosting is a bonus but not strictly required yet.

## Note 2: Job Hunt & Community
This section covers the mindset and non-technical strategies required for the upcoming job search ("Hunttober").

### Key Takeaways
Community is leverage: Engaging with the community is a "cheat code." Alumni have secured jobs simply by networking internally or helping others, without even applying.

Build in Public: Sharing your progress on platforms like LinkedIn and Twitter is non-negotiable. It increases visibility and can lead to recruiters reaching out directly.

Documentation is a Win: Documenting your learning journey and creating guides for new hires is an "easy win" when starting a new job, establishing you as a valuable team member early on.

Trust the Process: Success stories range from high school dropouts with employment gaps to those recovering from illness. Consistency and following the program (networking, Anki, daily coding) yield results.

The "Celebrations" Channel: Use this Discord channel as a data source. Read the detailed threads from hired students to understand the current market, interview questions, and successful strategies.

### 1. Tailwind CSS Setup
To avoid complex build steps (like installing via npm) for the MVP, the instructor utilized a "CDN" (Content Delivery Network) approach.


The Action: He grabbed a script tag from the Tailwind documentation and placed it inside the <head> of his HTML document.

The Code Structure:

HTML
<head>
  <script src="https://cdn.tailwindcss.com"></script>
</head>

Purpose: This allows the browser to read Tailwind utility classes (like flex, text-center, bg-blue-500) and style them instantly without setting up a development environment.

### 2. Tailwind Components (Hero & Feature Sections)

Instead of writing CSS from scratch, the instructor used pre-made "components" available on Tailwind's website or similar free resources.

The Hero Section:


Action: He located a "Hero" component (typically the large introductory section at the top of a webpage), copied the raw HTML code, and pasted it directly into the <body> tag.

Breakdown: This code consists of standard HTML elements (<div>, <h1>, <button>) heavily styled with Tailwind utility classes.

The Feature Section:


Action: He looked for a "feature section" (specifically one with a "join" theme), copied the HTML, and pasted it below the Hero section.


Result: The page instantly rendered a fully responsive layout with navigation, headings, and buttons without writing a single line of custom CSS.

3. DaisyUI Setup
DaisyUI was introduced as a tool that sits "on top" of Tailwind to provide higher-level components (like pre-styled buttons and footers) rather than just low-level utility classes.


The Action: The instructor grabbed the CDN link for DaisyUI and added it to the <head> of the document. He initially pasted it inside the wrong script tag but corrected it by placing it as a separate link/script.

### The Code Structure:

HTML
<head>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdn.jsdelivr.net/npm/daisyui@latest/dist/full.css" rel="stylesheet" type="text/css" />
</head>

4. DaisyUI Component (Footer)
The instructor used DaisyUI specifically to create a footer, highlighting how it simplifies the code compared to raw Tailwind.


The Action: He selected a "Footer" component from the DaisyUI documentation, copied the HTML, and pasted it at the bottom of his HTML body.

Breakdown: Unlike the Tailwind examples which might use 10+ classes to style a single element, DaisyUI often uses semantic component classes (e.g., footer, btn, card).


Result: Upon refreshing the browser, a fully styled, dark-themed footer appeared at the bottom of the page.

Summary of the "MVP Stack" Workflow
The specific workflow demonstrated was:


Setup: Drop CDN scripts for Tailwind and DaisyUI into the <head>.


Browse: Go to documentation sites (Tailwind UI or DaisyUI) and find visual components like "Hero," "Features," or "Footer".


Copy-Paste: Copy the HTML block provided and paste it into your index.html.


Run: Open the file in a browser to see a professional-looking site immediately.

### Key Takeaway: 
The instructor emphasized that for an MVP, you should not focus on how it looks or writing custom styles. Instead, "grab some components... and you're done".



---

## Class 01 | HTML basics
The following notes and summary are drawn from the transcript of the first class of the **#100Devs software engineering bootcamp**, which focuses on transitioning into a career in web development through structured learning and community support.

### **Summary**
The instructor emphasizes that while software engineering is a high-paying and happy career that does not require a degree, it is exceptionally difficult and requires a specific mindset to survive the **"Trough of Sorrow"**—the period where many learners give up. The class covers the basic mechanics of the internet (request/response cycles), the essential roles of HTML, CSS, and JavaScript, and scientifically proven study methods like **Active Recall** and **Spaced Repetition**.

### **The Web Development Workflow**
The sources define the technical and professional workflow for an aspiring developer as follows:

*   **The Technical Request-Response Cycle:**
    *   **The Client:** A device (phone, laptop) running a browser makes a request for information.
    *   **DNS (Domain Name Server):** Acts as a "phone book" that translates a URL (like facebook.com) into an IP address to locate the correct server.
    *   **The Server:** A computer that "serves" the requested files (HTML, CSS, and JavaScript) back to the client.
    *   **Rendering:** The browser opens these files to display the content (HTML), apply styling (CSS), and enable interaction (JavaScript).
*   **The Career Transition Workflow:**
    *   **Phase 1: Learn the basics** of front-end and back-end development.
    *   **Phase 2: Build** a large-scale passion project and freelance for real clients.
    *   **Phase 3: Network** aggressively while transitioning into "interview mode".

### **Essential Tools**
*   **Text Editors:** Recommended tools for writing code include **Atom**, **VS Code**, or **Sublime Text**.
*   **Browsers:** **Chrome** or **Firefox** are the preferred environments for testing and rendering web pages.
*   **Community & Materials:** **Discord** is used for hosting all starter code, slides, and peer support. **Twitter** is utilized for attendance "check-ins" and as a primary tool for professional networking.
*   **Learning & Retention:** 
    *   **Anki:** A flashcard app that uses an algorithm to automate **Spaced Repetition** and flatten the "forgetting curve".
    *   **Coursera:** Students are assigned the "Learning How to Learn" course to master study techniques.
*   **Version Control:** **GitHub** is the future destination for storing code and submitting homework via pull requests.

### **Guidelines**
*   **Separation of Concerns:** This is the "Golden Rule." Content must stay in HTML, styling in CSS, and behavior in JavaScript. Never mix them.
*   **Semantic HTML:** Choose HTML tags based on their **meaning and importance** (e.g., using an `<h1>` for the most important heading), not based on how they look in the browser.
*   **Networking Strategy:** The sources state that **"clicking apply is like lighting your resume on fire."** Instead, students must network their way into positions through "coffee chats" and referrals.
*   **Effective Study Habits:** Stop highlighting and rereading. Use **Active Recall** (quizzing yourself on material) and **Spaced Repetition** (reviewing at increasing intervals) to learn faster and retain information permanently.
*   **Frustration Management:** Success in coding is a reflection of how one handles being stuck. It is a marathon, and learners must prioritize **sleep and self-care** to consolidate knowledge.

### **Key Takeaways**
*   **Coding is Not Enough:** Learning the technical skill is the "easy" part; the hard part of getting a job is the **networking and interviewing**.
*   **Consistency is Vital:** You are better off doing **20 minutes of work every single day** than trying to cram for five hours once a week.
*   **Full-Stack Strategy:** The goal is to become a "Full Stack" developer, meaning you can handle both the **front-end** (client-side) and **back-end** (server-side) of an application.
*   **Security Matters:** Understand that **HTTPS** is the secure version of the transfer protocol that encrypts data between the client and server.
*   **Community Support:** Having a community to help you get "unstuck" is the primary factor that prevents learners from quitting.

---

## Class 02 | More about HTML
This session focuses on the structural layer of the web, emphasizing the relationship between clients and servers and the correct use of HTML tags. 

### Workflow:
- Active Engagement: Rather than passive re-watching, students are encouraged to engage with the material once and then apply it immediately. 
- Coding by Hand: Avoid shortcuts and plugins initially; type out all tags to build muscle memory and a deeper understanding of syntax. 
- Study Method: Use "Anki" (flashcards) for active recall, specifically focusing on short questions with detailed answers. 

### Tools:
- HTML: Used to power the structure and content of a webpage. 
- MDN (Mozilla Developer Network): A primary reference for looking up documentation and tag usage. 
- **Anki: A tool for space repetition to reinforce learning.**

### Guidelines:
- Separation of Concerns: Keep content (HTML), styling (CSS), and behavior (JavaScript) separate. 
- Semantic HTML: Use tags like <strong> and <em> instead of just bolding or italics because they provide meaning to screen readers and search engines. 
- **Accessibility: Code should be readable by general users, assistive devices, and search engines alike.**

### Key Takeaways:
- Master the syntax (spelling, grammar, and punctuation of code) to avoid common errors. 
- Understand the client-server model as the fundamental communication path of the web.

---
## Class 03 | CSS

This session transitions into the styling layer of web development, introducing CSS syntax and advanced learning strategies. 

### Workflow:
- Mastery-Based Learning: Do not move on to a new topic until the current one is fully mastered. 
- Debugging: When CSS breaks, check for missing semicolons, colons between properties/values, or unclosed curly braces. 
- Project Structure: Organize files clearly, such as keeping CSS files in a dedicated folder relative to the HTML file. 

### Tools:
- CSS: The technology used for coloring, styling, and making websites look good. 
- Atom Editor: A text editor used for writing and managing code files. 
- Discord: Used for community support and accessing learning materials. 

### Guidelines:
- Floats vs. Modern Layouts: Learn "floats" to understand legacy codebases, but prioritize Flexbox and Grid for modern development. 
- Specificity & !important: Use the !important tag only as a last resort in emergencies (e.g., during a client meeting) and fix the underlying specificity issue afterward. 
- Research First: Exhaustive research is expected before asking for help in community channels. 

### Key Takeaways:
- CSS follows a cascading nature; errors in one line can cause all subsequent styles to break.
- Deep learning and honesty with the material (e.g., through reading Shay Howe) are more effective than rushing.

---

#### Class 04 | CSS layout
#### Class 05 | More CSS layout
#### Class 06 | Responsive CSS
#### Class 07 | Code vomit 
#### Class 08 | More responsive CSS layout
#### Class 09 | JS basics
#### Class 10 | JS basics
#### Class 11 | More JS
#### Class 12 | Freelance
#### Class 13 | JS loops
#### Class 14 | The practice of JS loops
#### Class 15 | JS arrays 
#### Class 16 | JS objects
#### Class 17 | More JS objects
#### Class 18 | Reviewing JS objects
#### Class 19 | JS objects
#### Class 20 | APIs with JS
#### Class 21 | Git & github
#### Class 22 | JS Practice 
#### Class 23 | JS & APIs Practice 
#### Class 24 | JS
#### Class 25 | JS OOP
#### Class 26 | More JS OOP
#### Class 27 | Practical JS OOP
#### Class 28 | A job in tech part 1
#### Class 29 | A job in tech part 2
#### Class 30 | Node crash
#### Class 31 | JS event loop
#### Class 32 | API
#### Class 33 | APPs with Node & Express
#### Class 34 | CRUD APP with Node & Express
#### Class 35 | Reviewing CRUD APP with Node & Express
#### Class 36 | Todo list
#### Class 37 | Todo list follow MVC
#### Class 38 | Adding MS authentication to the Node APPs part 1
#### Class 39 | Adding MS authentication to the Node APPs part 2
#### Class 40 | Getting a job
#### Class 41 | Team project
#### Class 42 | Building Social network
#### Class 43 | Back-end crash
#### Class 44 | Back-end crash
#### Class 45 | Setting the end of program
#### Class 46 | Intro to React
#### Class 47 | Intro to React
#### Class 48 | Graduation
#### Class 49 | Interview
#### Class 50 | Interview
#### Class 51 | Adding ML projects to the portfolio
#### Class 52 | ML portfolio projects
#### Class 53 | The start of mega
#### Class 54-57 | Intro to data structures and algorithms
#### Class 58 | Big O notation
#### Class 59 | Getting a job in tech part 1
#### Class 60 | Getting a job in tech part 2
#### Class 61 | Getting a job in tech part 3
#### Class 62 | Blogging for developers
#### Class 63 | Getting a job as a software engineer
#### Class 64 | Fullstack Web Dev



### Web Dev Bootcamp
#### Class 1  | Web Dev
#### Class 2  | Web Dev
#### Class 3  | CSS
#### Class 4  | Web Dev
#### Class 5  | Back-end crash
#### Class 6  | Responsive CSS
#### Class 7  | Flexbox and JS
#### Class 8  | JS
#### Class 9  | JS
#### Class 10 | JS
#### Class 11 | JS animations
#### Class 12 | JS
#### Class 13 | JS arrays
#### Class 14 | JS objects


---
Ref:
100devs with Leon Noel

