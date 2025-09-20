# AI Development Enablement Workflow

This workflow outlines a proven, AI-augmented process for accelerating the product development lifecycle from ideation to delivery. This is a personal process that can be adapted to fit any team's needs.

[Flowchart illustrating the AI-augmented development process]

### Phase 1: AI-Powered Requirement Gathering and Definition

- **Step 1.1: Ideation & Scoping Session**
  - **Action:** Conduct a meeting with stakeholders to discuss the project vision. Record or take detailed notes.
  - **AI Integration:** Use a tool like **Gemini** to transcribe the meeting and generate a high-level summary. Pose questions to the AI to refine the project's scope.
  - **Prompt Example:** "Based on these notes, what are the key features? What questions should I ask to clarify the business goals and define the scope for a residential parking sharing platform?"
- **Step 1.2: Requirements Document Generation**
  - **Action:** Use the AI to generate a comprehensive requirements document.
  - **AI Integration:** With the context from the previous step, prompt the AI to create a document with an introduction, scope, high-level flow, and detailed user stories.
  - **Tool Links:** [Gemini](https://gemini.google.com/ "null"), [Jira](https://www.atlassian.com/software/jira "null"), [Trello](https://trello.com/ "null")
- **Step 1.3: Iterative Refinement**
  - **Action:** Review the generated document and provide feedback to the AI.
  - **AI Integration:** Continuously iterate by asking the AI to make changes, such as "Please rephrase the user stories for better clarity" or "Can you add a section on success metrics?"

### Phase 2: Rapid Prototyping & Front-End Development

- **Step 2.1: Prompt Engineering for Prototyping**
  - **Action:** Develop a precise prompt for a rapid prototyping tool.
  - **AI Integration:** Use **Gemini** to generate a V0-specific prompt. Instruct the AI to focus on key architectural patterns:
    - **Framework:** React
    - **Structure:** Component-based (not monolithic)
    - **Design:** Mobile-first approach
    - **Styling:** Tailwind CSS
    - **Theme:** Professional, inviting, and actionable design that fits the project's purpose.
- **Step 2.2: Prototype Generation & Iteration**
  - **Action:** Pass the refined prompt to **V0** to generate the front-end code.
  - **AI Integration:** Download the code and, if needed, provide feedback to V0 for design or structural changes until you are satisfied with the result.
  - **Tool Links:** [V0](https://v0.dev/ "null")
- **Step 2.3: Local Development & Functional Mocking**
  - **Action:** Open the downloaded code in a local editor and make it runnable.
  - **AI Integration:** Use a tool like **Cursor** to analyze the project. Ask the AI to:
    - Make the codebase runnable locally.
    - Make the front-end UI navigable and functional.
    - Mock data to simulate a live application. This is a highly iterative step.
  - **Tool Link:** [Cursor](https://cursor.sh/ "null")

### Phase 3: Deployment & User Validation

- **Step 3.1: Code Versioning**
  - **Action:** Upload the functional front-end code to a version control system.
  - **AI Integration:** Ensure the code is properly structured and well-commented before committing.
  - **Tool Link:** [GitHub](https://github.com/ "null")
- **Step 3.2: Continuous Deployment**
  - **Action:** Connect the GitHub repository to a deployment service.
  - **AI Integration:** **Netlify** automatically deploys the site, providing a live URL for a client demo.
  - **Tool Link:** [Netlify](https://www.netlify.com/ "null")
- **Step 3.3: Demo & Feedback Loop**
  - **Action:** Present the live demo to the client.
  - **AI Integration:** Capture client feedback and use it as a basis for the next AI-assisted iteration, repeating the prototyping and local development steps until the client is satisfied.

### Phase 4: Backend & Test Automation

- **Step 4.1: Documentation Generation**
  - **Action:** Generate documentation for the project.
  - **AI Integration:** Use **Cursor** to analyze the entire project and generate markdown documentation (`.md`) files. This includes instructions for local setup, project architecture, and a user-facing site map or guide.
- **Step 4.2: Backend Development**
  - **Action:** Build the backend logic and database.
  - **AI Integration:** Use **Cursor** to assist with backend development, connecting to services like **Supabase** . Request one feature or endpoint at a time to avoid errors. **Note:** Define and enforce "AI rules" or best practices (e.g., from [Kotlin Docs](https://kotlinlang.org/docs/home.html "null")) to ensure clean, consistent code.
  - **Tool Link:** [Supabase](https://supabase.com/ "null")
- **Step 4.3: Automated Testing**
  - **Action:** Generate and integrate automated tests.
  - **AI Integration:** With **Cursor** or **Copilot** , ask the AI to generate Cypress tests. Provide detailed instructions for:
    - Installation
    - Project structure (`e2e`, `component`, etc.)
    - Selector assignment
    - Test report generation
    - Test coverage review
    - Evidence generation
    - CI/CD integration for automated regression.
  - **Tool Links:** [Cypress](https://www.cypress.io/ "null"), [Copilot](https://github.com/features/copilot "null")
