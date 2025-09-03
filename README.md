# Assignment-5

1. Creating a Reusable Custom Hook (useFetch)

Decision:
To avoid repetitive fetch logic across components, a custom hook useFetch was created to handle API data fetching, loading states, and error handling.

Why:
This simplifies the code and promotes reusability, separation of concerns, and cleaner component files.

2. Hook Structure and API Handling

Decision:
The hook uses:

useState to manage data, loading, and error states.

useEffect to trigger the fetch when the component mounts or when the URL changes.

fetch API for simplicity and browser-native support.

Why:
These React hooks are well-suited for side effects (like fetching) and managing async state changes.

3. Loading and Error Handling

Decision:
Implemented conditional rendering in the component to show:

A loading spinner or message when data is being fetched.

An error message if the request fails.

Why:
This improves user experience and helps with debugging or slow networks.

4. Flexible API Usage

Decision:
The useFetch hook is generic and works with any valid URL, not just a specific API.

Why:
Makes the hook more reusable across different parts of a project or even across different projects.

5. Component Design

Decision:
A simple UI component was created to:

Display product information fetched from https://api.escuelajs.co/api/v1/products.

Keep the focus on the hook functionality.

Why:
Keeps the codebase clean and highlights the power of the custom hook.

6. Code Deployment and Versioning

Decision:

Deployed to Netlify for easy access and demonstration.

Pushed the code to GitHub for version control and submission.

Why:
Standard practice for frontend projects and meets submission requirements.

7. Styling Decisions

Decision:
Minimal CSS styling was applied to ensure readability and clean UI presentation.

Why:
The main focus is on the hook functionality rather than complex UI at this stage.
