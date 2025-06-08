# React Interview Mental Models & Strategic Patterns

## **PATTERN RECOGNITION TRIGGERS**

### **When You Hear These Keywords → Think This Pattern**

#### **"Performance" / "Slow" / "Re-render" → React Performance Audit Pattern**
- **Trigger Words**: "laggy", "many components", "expensive operations"
- **Mental Framework**:
  - Identify what's causing re-renders
  - Check: Props changes, State changes, Parent re-renders, Context changes
  - Solutions: React.memo, useMemo, useCallback, state colocation

#### **"State" / "Data Flow" / "Communication" → React State Flow Pattern**
- **Trigger Words**: "share data", "component communication", "global state"
- **Mental Framework**:
  - Local state → Lift state up → Context → External state management
  - Always choose the least complex solution first

#### **"Lifecycle" / "Mounting" / "Effect" → Hook Lifecycle Mapping**
- **Trigger Words**: "componentDidMount", "cleanup", "side effects"
- **Mental Framework**:
  - Class lifecycle → Hook equivalent
  - Always think: When does this run? What does it depend on? How to cleanup?

#### **"Render" / "Update" / "DOM" → React Render Cycle Pattern**
- **Trigger Words**: "rendering", "virtual DOM", "reconciliation"
- **Mental Framework**:
  - Trigger → Render → Reconcile → Commit
  - Understand what triggers renders and how to optimize

---

## **REACT-SPECIFIC MENTAL MODELS**

### **The "Component Hierarchy Visualizer"**
```
Question Pattern: State management, prop passing, communication

Mental Framework:
Parent Component
├── Child A (needs data)
├── Child B (has data)
└── Child C (needs data)

Solutions hierarchy:
1. Lift state to common parent
2. Use Context if deeply nested
3. External state if complex
```

### **The "Re-render Debugger"**
```
Question Pattern: "Why is this component re-rendering?"

Mental Framework:
1. Parent re-rendered?
2. Props changed?
3. State changed?
4. Context value changed?
5. Force re-render called?

Always trace the source of the re-render
```

### **The "Hook Dependency Tracker"**
```
Question Pattern: useEffect, useCallback, useMemo dependency questions

Mental Framework:
1. What values from component scope am I using?
2. Do these values change between renders?
3. Do I want the hook to re-run when they change?
4. ESLint exhaustive-deps rule compliance
```

### **The "State vs Props Classifier"**
```
When to use State:
- Data changes over time
- Controlled by this component
- Triggers re-renders

When to use Props:
- Data from parent
- Read-only in this component
- Configuration/data passing
```

---

## **COMPONENT DESIGN MENTAL MODELS**

### **The "Single Responsibility Principle for Components"**
```
Question: "How would you structure this component?"

Mental Framework:
1. What is the component's single responsibility?
2. Can it be broken into smaller components?
3. What data does it need vs what should it receive?
4. Is it presentational or contains business logic?
```

### **The "Composition vs Inheritance Decider"**
```
React Pattern: Favor composition over inheritance

Mental Framework:
Instead of: Component inheritance
Use: Higher-order components, Render props, Hooks, Component composition
```

### **The "Smart vs Dumb Component Pattern"**
```
Smart (Container) Components:
- Handle state and logic
- Connect to external data
- Manage side effects

Dumb (Presentational) Components:
- Receive props and render
- No internal state (except UI state)
- Reusable and testable
```

---

## **PERFORMANCE OPTIMIZATION PATTERNS**

### **The "React Performance Checklist"**
```
Performance Issue Triggers:
1. Unnecessary re-renders → React.memo, useMemo, useCallback
2. Expensive computations → useMemo
3. Large lists → Virtualization
4. Bundle size → Code splitting, lazy loading
5. Initial load → SSR/SSG
```

### **The "Memoization Decision Tree"**
```
Should I memoize?

Expensive computation → useMemo
Function passed to child → useCallback
Component props rarely change → React.memo
Complex object/array → useMemo for reference equality
```

### **The "Re-render Prevention Strategy"**
```
1. Move state down (state colocation)
2. Separate contexts
3. Memoize components (React.memo)
4. Memoize values (useMemo)
5. Memoize callbacks (useCallback)
6. Use state updater functions
```

---

## **HOOK PATTERN RECOGNITION**

### **The "Hook Selection Matrix"**
```
Simple state → useState
Complex state logic → useReducer
Side effects → useEffect
Layout effects → useLayoutEffect
Referencing DOM → useRef
Expensive calculations → useMemo
Stable function reference → useCallback
Context consumption → useContext
```

### **The "useEffect Pattern Matcher"**
```
No dependency array → Runs after every render
Empty dependency array → Runs once (componentDidMount)
With dependencies → Runs when dependencies change
Return cleanup function → componentWillUnmount equivalent
```

### **The "Custom Hook Identifier"**
```
Create custom hook when:
- Logic is reused across components
- Complex stateful logic
- Side effect abstraction
- Third-party library integration
```

---

## **STATE MANAGEMENT DECISION TREE**

### **The "State Management Escalation Ladder"**
```
1. Local useState/useReducer
2. Lift state up to common parent
3. React Context (for sharing, not frequent updates)
4. External state management (Redux, Zustand, etc.)

Choose based on:
- Complexity of state logic
- Number of components needing access
- Frequency of updates
- Team size and expertise
```

### **The "Context Performance Pattern"**
```
Context Performance Issues:
- Every context change re-renders all consumers
- Split contexts by update frequency
- Memoize context values
- Use multiple contexts instead of one large context
```

---

## **ERROR HANDLING PATTERNS**

### **The "Error Boundary Strategy"**
```
Question: "How do you handle errors in React?"

Mental Framework:
1. Error boundaries for component tree errors
2. try-catch for event handlers and async code
3. Graceful degradation
4. Error reporting/logging
5. User-friendly error messages
```

### **The "Async Error Handling Pattern"**
```
useEffect with async:
- Don't make useEffect callback async
- Handle promise rejections
- Check if component is still mounted
- Use AbortController for cleanup
```

---

## **TESTING MENTAL MODELS**

### **The "React Testing Philosophy"**
```
Test behavior, not implementation:
- Test what users see and do
- Mock external dependencies
- Test component contracts (props in, rendered output)
- Test user interactions
```

### **The "Testing Strategy Pyramid"**
```
Unit Tests: Individual components/hooks
Integration Tests: Component groups working together
E2E Tests: Full user workflows

Focus on integration tests for React apps
```

---

## **INTERVIEW CONVERSATION PATTERNS**

### **The "React Deep Dive Anticipation"**
```
When you mention any React concept, expect:
"How would you implement this hook from scratch?"
"What are the performance implications?"
"How would you test this?"
"What happens if the component unmounts?"
"How does this work with Concurrent React?"
```

### **The "Component Design Progression"**
```
Basic functional component
↓
Add state with hooks
↓
Handle side effects
↓
Optimize performance
↓
Add error handling
↓
Make it reusable
↓
Add testing
```

---

## **SPECIFIC REACT TRIGGER-RESPONSE PATTERNS**

### **Lifecycle Method Triggers**
- **Hear**: "componentDidMount", "componentWillUnmount", "lifecycle"
- **Think**: Hook equivalents, effect dependencies, cleanup
- **Pattern**: Map old lifecycle to useEffect patterns

### **State Management Triggers**
- **Hear**: "global state", "prop drilling", "share data"
- **Think**: State management escalation ladder
- **Pattern**: Start simple, escalate complexity as needed

### **Performance Triggers**
- **Hear**: "slow", "many components", "expensive"
- **Think**: Re-render causes, memoization opportunities
- **Pattern**: Profile first, then optimize specific bottlenecks

### **Hook Triggers**
- **Hear**: "custom logic", "reusable", "stateful logic"
- **Think**: Custom hook extraction
- **Pattern**: Identify reusable stateful logic patterns

---

## **RAPID RESPONSE CHEAT PATTERNS**

### **For "What happens when..." React questions**
1. Trace the render cycle
2. Identify what triggers the render
3. Follow the reconciliation process
4. Note side effects and cleanup

### **For "How would you optimize..." questions**
1. Identify the performance bottleneck
2. Apply appropriate memoization
3. Consider architectural changes
4. Discuss measurement and monitoring

### **For "How would you structure..." questions**
1. Start with component responsibility
2. Consider data flow
3. Plan for scalability
4. Apply React patterns

### **For Hook-related questions**
1. Identify the hook's purpose
2. Consider dependencies and effects
3. Think about cleanup
4. Consider custom hook extraction

---

## **ADVANCED REACT PATTERNS RECOGNITION**

### **Render Prop Pattern Recognition**
```
When you need:
- Flexible component logic sharing
- Dynamic rendering based on state
- Inversion of control

Pattern: Component with function as children or prop
```

### **HOC Pattern Recognition**
```
When you need:
- Cross-cutting concerns (auth, logging)
- Props manipulation
- Component enhancement

Pattern: Function that takes component, returns enhanced component
```

### **Compound Component Pattern Recognition**
```
When you need:
- Related components working together
- Flexible component composition
- Implicit state sharing

Pattern: Parent component with specialized children components
```

---

## **REACT 18+ SPECIFIC PATTERNS**

### **Concurrent Features Recognition**
```
useTransition → For non-urgent state updates
useDeferredValue → For expensive re-renders
Suspense → For data fetching and code splitting
```

### **Server Components Pattern**
```
When you see: "server components", "RSC"
Think: 
- Rendering location (server vs client)
- Data fetching implications
- Bundle size impact
- Hydration considerations
```

---

## **DEBUGGING MENTAL SHORTCUTS**

### **React DevTools Navigation**
```
Performance issues → Profiler tab
State/props debugging → Components tab
Hook debugging → Components tab, hook values
Re-render causes → Profiler, highlight updates
```

### **Common React Bugs Pattern**
```
Infinite re-render → Check useEffect dependencies
Stale closure → Check if using latest values
Memory leak → Check cleanup in useEffect
Hydration mismatch → Check server/client differences
```

---

## **INTERVIEW DAY EXECUTION FOR REACT**

### **First response to any React question:**
1. Clarify the React version/context
2. Identify core React concepts involved
3. Choose appropriate mental model
4. Consider performance implications from start

### **Always follow up React answers with:**
- "Here's how I'd test this..."
- "For performance, I'd consider..."
- "In a production app, I'd also..."
- "The trade-offs of this approach are..."

This React-specific pattern recognition transforms you from someone who knows React syntax to someone who thinks in React patterns and can architect scalable applications.
