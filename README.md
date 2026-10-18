# CS360-Mobile-Architecture

### 1. Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The primary goal of EventPulse was to deliver a secure, functional, and user-friendly mobile application designed to streamline personal and professional scheduling. The application requirements included implementing user authentication (login and account registration) backed by a persistent local SQLite database, interactive event management capabilities, and automated notification triggers. It was designed to address the common user need for a reliable, offline-capable productivity tool that allows individuals to effortlessly manage their schedules, maintain organized event logs, and securely handle their credentials without data loss.

### 2. What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
To support user needs, the app featured a streamlined Login/Registration screen (`LoginActivity`) and a primary dashboard screen (`MainActivity`) housing the event management interface. These screens kept users in mind by utilizing clean layouts, intuitive button mapping, and clear text input fields that minimized friction during onboarding and daily use. The designs were successful because they established a consistent visual hierarchy, reducing cognitive load and ensuring that core actions—such as creating an account, logging in, and navigating event grids—could be executed quickly and efficiently.

### 3. How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
My coding approach relied on a structured, modular, and database-first strategy. Before building out complex UI logic, I prioritized establishing a stable data layer using SQLite helper classes and robust schema constants to handle CRUD operations smoothly. I also utilized defensive programming techniques—such as validating user form inputs and handling runtime system permissions gracefully. In future projects, these strategies can be applied to ensure scalable database management, prevent runtime crashes, and maintain predictable application states.

### 4. How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
Testing was conducted rigorously using the Android Emulator across multiple virtual device configurations. This process is critical because it validates component lifecycles, verifies that database queries execute without errors, and ensures that UI layouts respond correctly under different conditions. Testing revealed minor method signature mismatches and button ID mapping discrepancies early in the development cycle, allowing me to resolve them before final deployment and ensuring seamless execution.

### 5. Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
One major challenge arose during the database wiring phase when synchronizing user account registration logic with the existing login input fields. To overcome this without complicating the user experience, I innovated by designing a unified database helper method that securely handles both account creation and credential verification within the same streamlined UI components, maintaining simplicity for the end user while ensuring backend integrity.

### 6. In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I was particularly successful in demonstrating my technical skills within the SQLite database helper implementation and activity lifecycle management. Successfully bridging Java-based UI activities with persistent local data storage—while properly managing runtime permissions like `SEND_SMS` and ensuring fallback behaviors—showcased a comprehensive understanding of secure, reliable mobile architecture.

### AI Usage Acknowledgment
Generative AI tools were utilized to assist with structuring and refining the technical documentation, app launch plan, and reflective writing components for this portfolio submission.
