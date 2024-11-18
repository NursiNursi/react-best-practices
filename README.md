# React Best Practices

Contain 17 React best practices


## 1. Constants / Harc-coded values / Magic Values

It's a better practice to define the hardcoded values somewhere else to easier to manage. Define those outside the component, typically these are written in capital case. It would be even easier to manage if we actually put this in a dedicated file named constants.js(inside a folder named "lib")

## 2. Folder Structure

There are no strict rules about folder structure, so don't worry too much about it. However, as a best practice, ensure it's easy for a new person to understand. Consistency is key, organize things by their semantic purpose. For example, components should be distinct from state management, and state management should be separate from constants and types. By keeping these elements distinct and organizing them differently, you can create a more intuitive structure.

## 3. Components: when to create them

Don't be afraid to create components as a best practice try to identify opportunities for reuse as well as when some element in the UI is distinct from something else.

## 4. Avoid unnecessary markup (div's)

Adding unnecessary div elements can clutter the HTML structure, potentially breaking the layout. Layout styling with Flexbox or CSS Grid depends on the HTML structure, so inserting a div may cause layout issues. Instead, consider using the React Fragment, which preserves the layout by not adding extra elements to the HTML.

## 5. Don't add layout styles to reusable component

As a best practice try not adding layout styles to your reusable component, instead if you need some kind of layout style just use one of a div or use the className prop.

## 6. Use TypeScript

TypeScript makes you code a little bit more strict, helping you catch mistakes more quickly and providing IntelliSense. It warns you when you've made an error and offers useful IntelliSense information to assist you when you're unsure about something.

## 7. Keep components simple (children pattern, updater function for useState)

Ensure your components, especially those lower in the component tree or those intended for reuse, remain simple and uncomplicated. Keeping them 'dumb' improves their reusability. If you have some kind of calculation typically you want to derive it just very close to where you actually have the original state instead of somewhere down in your component tree. And then you can just pass that as a prop.
