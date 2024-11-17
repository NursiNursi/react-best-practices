# React Best Practices

Contain 17 React best practices


## 1. Constants / Harc-coded values / Magic Values

It's a better practice to define the hardcoded values somewhere else to easier to manage. Define those outside the component, typically these are written in capital case. It would be even easier to manage if we actually put this in a dedicated file named constants.js(inside a folder named "lib")

## 2. Folder Structure

There are no strict rules about folder structure, so don't worry too much about it. However, as a best practice, ensure it's easy for a new person to understand. Consistency is key, organize things by their semantic purpose. For example, components should be distinct from state management, and state management should be separate from constants and types. By keeping these elements distinct and organizing them differently, you can create a more intuitive structure.
