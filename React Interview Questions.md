# React Interview Questions - Beginner to Advanced

## **REACT FUNDAMENTALS**

### Components & JSX
- What is React and why was it created?
- What is JSX and how does it work?
- What is the difference between React elements and components?
- What is the Virtual DOM and how does it work?
- What is the difference between functional and class components?
- What are React fragments and why use them?
- What is the difference between `<div>` and `<React.Fragment>`?
- How do you render lists in React?
- What is the importance of keys in React lists?
- What happens if you don't provide keys in lists?
- What are the rules for JSX?
- Can you return multiple elements from a component?
- What is the difference between HTML and JSX attributes?
- How do you write comments in JSX?
- What is JSX transpilation?

### Props & State
- What are props in React?
- What is state in React?
- What is the difference between props and state?
- How do you pass data between components?
- What is prop drilling?
- What are default props?
- What is prop validation and PropTypes?
- Can you modify props inside a component?
- What is the children prop?
- How do you pass functions as props?
- What is the difference between controlled and uncontrolled components?
- What is lifting state up?
- What is state colocation?

## **REACT HOOKS**

### Basic Hooks
- What are React Hooks?
- What are the rules of hooks?
- What is useState hook?
- What is useEffect hook?
- What is useContext hook?
- What is the difference between useState and useReducer?
- When should you use useReducer over useState?
- What is the dependency array in useEffect?
- What happens when you omit the dependency array?
- What happens when you pass an empty dependency array?
- How do you cleanup in useEffect?
- What is the difference between useEffect and useLayoutEffect?

### Advanced Hooks
- What is useCallback hook?
- What is useMemo hook?
- What is useRef hook?
- What is useImperativeHandle hook?
- What is useDebugValue hook?
- What is useDeferredValue hook?
- What is useTransition hook?
- What is useId hook?
- What is useSyncExternalStore hook?
- What is useInsertionEffect hook?
- How do you create custom hooks?
- What are the benefits of custom hooks?
- How do you test custom hooks?

### Hook Patterns
- What is the difference between useCallback and useMemo?
- When should you use useCallback?
- When should you use useMemo?
- What is the exhaustive deps rule?
- How do you handle async operations in useEffect?
- How do you fetch data with hooks?
- How do you handle race conditions with hooks?
- What is the stale closure problem?
- How do you share state between components with hooks?
- What is the useState functional update pattern?

## **COMPONENT LIFECYCLE**

### Class Component Lifecycle
- What are the phases of React component lifecycle?
- What is componentDidMount?
- What is componentDidUpdate?
- What is componentWillUnmount?
- What is shouldComponentUpdate?
- What is getSnapshotBeforeUpdate?
- What is componentDidCatch?
- What is getDerivedStateFromProps?
- What is getDerivedStateFromError?
- What are the deprecated lifecycle methods?

### Functional Component Lifecycle
- How do you replicate componentDidMount with hooks?
- How do you replicate componentDidUpdate with hooks?
- How do you replicate componentWillUnmount with hooks?
- How do you replicate shouldComponentUpdate with hooks?
- How do you handle errors in functional components?

## **EVENT HANDLING**

### Synthetic Events
- What are synthetic events in React?
- What is the difference between synthetic events and native events?
- What is event pooling?
- How do you access the native event?
- What is event delegation in React?
- How do you prevent default behavior in React?
- How do you stop event propagation in React?
- What is the difference between onClick and onClickCapture?

### Event Patterns
- How do you handle form submissions in React?
- How do you handle input changes in React?
- How do you debounce events in React?
- How do you handle keyboard events in React?
- How do you handle mouse events in React?
- How do you handle touch events in React?

## **FORMS & VALIDATION**

### Form Handling
- What are controlled components?
- What are uncontrolled components?
- When should you use controlled vs uncontrolled components?
- How do you handle form validation in React?
- What is the ref attribute?
- How do you focus an input in React?
- How do you handle file uploads in React?
- How do you handle multiple form inputs?
- What is the difference between value and defaultValue?

### Form Libraries
- What are popular form libraries for React?
- What is Formik?
- What is React Hook Form?
- What are the advantages of using form libraries?

## **STATE MANAGEMENT**

### Local State Management
- What are different ways to manage state in React?
- What is component state?
- What is application state?
- What is the difference between local and global state?
- How do you share state between sibling components?
- What is state normalization?

### Context API
- What is React Context?
- When should you use Context?
- What are the performance implications of Context?
- How do you optimize Context performance?
- What is the provider pattern?
- How do you use multiple contexts?
- What is context composition?

### External State Management
- What is Redux?
- What are the three principles of Redux?
- What is the difference between Redux and Context?
- What is MobX?
- What is Zustand?
- What is Recoil?
- What is Jotai?
- What is Valtio?
- When should you use external state management?

## **PERFORMANCE OPTIMIZATION**

### React Performance
- What causes re-renders in React?
- How do you prevent unnecessary re-renders?
- What is React.memo?
- What is PureComponent?
- What is the difference between React.memo and useMemo?
- How do you profile React applications?
- What is the React DevTools Profiler?
- What are performance bottlenecks in React?

### Optimization Techniques
- What is code splitting in React?
- What is lazy loading in React?
- What is React.lazy?
- What is Suspense?
- How do you implement error boundaries?
- What is server-side rendering (SSR)?
- What is static site generation (SSG)?
- What is incremental static regeneration (ISR)?
- What is the difference between SSR and SSG?

### Bundle Optimization
- How do you analyze bundle size?
- What is tree shaking?
- How do you reduce bundle size?
- What is webpack bundle analyzer?
- How do you implement preloading?
- How do you implement prefetching?

## **ROUTING**

### React Router
- What is React Router?
- What is the difference between BrowserRouter and HashRouter?
- What is the difference between Route and Switch?
- What are route parameters?
- What are query parameters?
- How do you handle nested routes?
- How do you implement protected routes?
- How do you handle redirects?
- What is programmatic navigation?
- What are route guards?

### Navigation Patterns
- How do you handle navigation in React?
- What is the history object?
- How do you navigate between routes programmatically?
- How do you handle back button functionality?
- How do you implement breadcrumbs?

## **STYLING**

### CSS in React
- How do you style React components?
- What is CSS-in-JS?
- What are the different ways to apply styles in React?
- What is the difference between inline styles and CSS classes?
- What are CSS modules?
- What is styled-components?
- What is emotion?
- What are the pros and cons of CSS-in-JS?

### Styling Libraries
- What is Material-UI?
- What is Ant Design?
- What is Chakra UI?
- What is Tailwind CSS with React?
- How do you implement theming in React?
- How do you handle responsive design in React?

## **TESTING**

### Testing Fundamentals
- How do you test React components?
- What is React Testing Library?
- What is Enzyme?
- What is the difference between shallow and mount rendering?
- How do you test hooks?
- How do you test custom hooks?
- How do you mock functions in tests?
- How do you test async components?

### Testing Patterns
- What is unit testing in React?
- What is integration testing in React?
- What is end-to-end testing in React?
- How do you test user interactions?
- How do you test form submissions?
- How do you test API calls?
- How do you test error boundaries?
- How do you test context providers?

### Testing Tools
- What is Jest?
- What is Cypress?
- What is Playwright?
- What is Storybook?
- How do you set up testing in React?
- What are testing best practices?

## **ADVANCED REACT PATTERNS**

### Component Patterns
- What is the render prop pattern?
- What are higher-order components (HOCs)?
- What is the compound component pattern?
- What is the provider pattern?
- What is the container/presentational pattern?
- What is the custom hook pattern?
- What is component composition?
- What is the children as function pattern?

### Advanced Concepts
- What is React Fiber?
- What is concurrent rendering?
- What is time slicing?
- What is the React reconciliation algorithm?
- What is the diffing algorithm?
- What are React portals?
- What is forward ref?
- What is React.cloneElement?
- What is React.Children?

## **REACT 18 FEATURES**

### New Features
- What is automatic batching?
- What are transitions?
- What is concurrent rendering?
- What is Suspense for data fetching?
- What is the new Suspense API?
- What is streaming SSR?
- What is selective hydration?
- What is the new strict mode behavior?

### New Hooks
- What is useTransition?
- What is useDeferredValue?
- What is useId?
- What is useSyncExternalStore?
- What is useInsertionEffect?

## **SERVER-SIDE RENDERING**

### SSR Concepts
- What is server-side rendering?
- What are the benefits of SSR?
- What are the challenges of SSR?
- What is hydration?
- What is the hydration mismatch?
- How do you handle client-server differences?
- What is progressive enhancement?

### SSR Frameworks
- What is Next.js?
- What is Gatsby?
- What is Remix?
- What are the differences between these frameworks?
- How do you choose between SSR frameworks?

## **REACT NATIVE**

### React Native Basics
- What is React Native?
- What is the difference between React and React Native?
- What is the bridge in React Native?
- What are native components?
- What is the Virtual DOM in React Native?
- How do you handle navigation in React Native?
- How do you handle state management in React Native?

### React Native Patterns
- What is the difference between View and div?
- What is the difference between Text and span?
- How do you handle styling in React Native?
- How do you handle platform-specific code?
- How do you handle device orientation?
- How do you handle keyboard events?

## **DEBUGGING & DEVELOPMENT TOOLS**

### Debugging
- How do you debug React applications?
- What are React Developer Tools?
- How do you use the React Profiler?
- How do you debug performance issues?
- How do you debug memory leaks?
- How do you debug re-renders?
- What is the React error boundary?

### Development Tools
- What is Hot Module Replacement (HMR)?
- What is Fast Refresh?
- How do you set up a React development environment?
- What is Create React App?
- What is Vite?
- What is Webpack?
- How do you eject from Create React App?

## **ARCHITECTURE & BEST PRACTICES**

### Component Architecture
- How do you structure a React application?
- What is component hierarchy?
- How do you organize your components?
- What are smart and dumb components?
- How do you handle prop drilling?
- What is component composition vs inheritance?
- How do you design reusable components?

### Best Practices
- What are React best practices?
- How do you handle error boundaries?
- How do you optimize bundle size?
- How do you handle code splitting?
- How do you implement progressive web apps with React?
- How do you handle accessibility in React?
- How do you implement internationalization?

## **DATA FETCHING**

### Data Fetching Patterns
- How do you fetch data in React?
- What are the different data fetching patterns?
- How do you handle loading states?
- How do you handle error states?
- How do you handle race conditions?
- How do you implement caching?
- How do you handle pagination?

### Data Fetching Libraries
- What is React Query (TanStack Query)?
- What is SWR?
- What is Apollo Client?
- What is Relay?
- What are the benefits of using data fetching libraries?
- How do you choose between data fetching libraries?

## **SECURITY**

### React Security
- What are common security vulnerabilities in React?
- How do you prevent XSS attacks in React?
- How do you sanitize user input?
- What is dangerouslySetInnerHTML?
- How do you handle authentication in React?
- How do you handle authorization in React?
- How do you store sensitive data in React?

## **DEPLOYMENT & PRODUCTION**

### Build & Deployment
- How do you build a React application for production?
- What is the difference between development and production builds?
- How do you deploy React applications?
- What are environment variables in React?
- How do you handle different environments?
- What is continuous integration/deployment with React?

### Production Optimization
- How do you optimize React applications for production?
- What is service worker in React?
- How do you implement caching strategies?
- How do you handle SEO with React?
- How do you monitor React applications in production?
- How do you handle errors in production?

## **MICRO-FRONTENDS**

### Micro-frontend Architecture
- What are micro-frontends?
- How do you implement micro-frontends with React?
- What are the benefits and challenges of micro-frontends?
- How do you share state between micro-frontends?
- How do you handle routing in micro-frontends?
- What is Module Federation?

## **REACT ECOSYSTEM**

### Popular Libraries
- What are the most popular React libraries?
- What is React Router?
- What is Redux Toolkit?
- What is Framer Motion?
- What is React Spring?
- What is React Hook Form?
- What is React Table?
- What is React DnD?

### Development Ecosystem
- What is the React ecosystem?
- How do you choose React libraries?
- What is npm vs yarn?
- What is package-lock.json?
- How do you handle dependency management?
- What is semantic versioning?

## **CODING CHALLENGES**

### Component Implementation
- Implement a counter component
- Implement a todo list
- Implement a search component with debouncing
- Implement a pagination component
- Implement a modal component
- Implement a dropdown component
- Implement a carousel component
- Implement a drag and drop component

### Hook Implementation
- Implement useState from scratch
- Implement useEffect from scratch
- Implement useCallback from scratch
- Implement useMemo from scratch
- Implement a custom useLocalStorage hook
- Implement a custom useFetch hook
- Implement a custom useDebounce hook
- Implement a custom useThrottle hook

### State Management
- Implement a simple Redux
- Implement Context with useReducer
- Implement a shopping cart
- Implement a form with validation
- Implement undo/redo functionality
- Implement optimistic updates

### Performance Optimization
- Optimize a slow rendering component
- Implement virtual scrolling
- Implement lazy loading
- Implement code splitting
- Optimize bundle size
- Fix memory leaks

### Architecture Problems
- Design a component library
- Design a data fetching layer
- Design a routing system
- Design a state management solution
- Design a theming system
- Design a form builder

## **SYSTEM DESIGN (React Focus)**

### Frontend Architecture
- How would you architect a large React application?
- How do you handle state management at scale?
- How do you implement micro-frontends?
- How do you handle code sharing between teams?
- How do you implement a design system?
- How do you handle performance at scale?

### Real-world Scenarios
- Design a chat application
- Design a social media feed
- Design an e-commerce platform
- Design a dashboard application
- Design a collaborative editor
- Design a video streaming platform

## **MIGRATION & LEGACY**

### Migration Strategies
- How do you migrate from class components to hooks?
- How do you migrate from older React versions?
- How do you migrate from other frameworks to React?
- How do you handle breaking changes?
- How do you implement feature flags?
- How do you handle backward compatibility?

### Legacy Integration
- How do you integrate React with legacy applications?
- How do you gradually adopt React?
- How do you handle jQuery with React?
- How do you handle server-rendered content?
- How do you handle third-party libraries?
