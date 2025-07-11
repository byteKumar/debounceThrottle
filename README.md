# Debouncing and Throttling Examples

This repository contains practical examples demonstrating two important JavaScript performance optimization techniques: **Debouncing** and **Throttling**. These techniques are essential for handling high-frequency events like user input, scroll events, and API calls efficiently.

## 📁 Files Overview

### 1. example1.html - Debouncing Implementation
This file demonstrates various debouncing techniques for optimizing user input handling.

**Features:**
- **Trailing Debounce**: Executes the function only after the user stops typing for the specified delay
- **Leading Debounce**: Executes the function immediately on the first event, then ignores subsequent events during the delay period
- **Combined Debounce**: Executes on both leading and trailing edges of the event sequence

**Use Case:** Perfect for search input fields where you want to make API calls only after the user finishes typing, reducing unnecessary server requests.

**Implementation Details:**
- Input field with real-time event listening
- Three different debouncing strategies
- 2-second delay for demonstration
- Console logging to track API call simulation

### 2. example2.html - Throttling Implementation
This file showcases different throttling approaches for rate-limiting function execution.

**Features:**
- **Advanced Throttle**: Configurable leading and trailing execution options
- **Leading Throttle**: Executes immediately on first call, then blocks subsequent calls for the delay period
- **Trailing Throttle**: Delays execution and always uses the latest arguments

**Use Case:** Ideal for scroll events, resize handlers, or any scenario where you need to limit function execution frequency while maintaining responsiveness.

**Implementation Details:**
- Input field for testing throttle behavior
- Multiple throttling strategies with different execution patterns
- 1-second delay for demonstration
- Flexible options for leading/trailing execution

## 🚀 How to Use

1. **Clone or download** this repository
2. **Open either HTML file** in your web browser
3. **Open browser developer tools** (F12) to view console output
4. **Type in the input field** to see the debouncing/throttling effects in action

## 🔍 Key Differences

| Technique | When to Use | Behavior |
|-----------|-------------|----------|
| **Debouncing** | Search inputs, form validation | Waits for pause in events before executing |
| **Throttling** | Scroll events, resize handlers | Limits execution frequency regardless of event frequency |

## 💡 Learning Outcomes

After exploring these examples, you'll understand:
- How to implement debouncing for input optimization
- Different throttling strategies and their use cases
- When to choose debouncing vs throttling
- Performance benefits in real-world applications
- How to handle high-frequency DOM events efficiently

## 🛠 Technical Implementation

Both examples include:
- Clean, modern HTML structure
- CSS styling for better user experience
- Multiple implementation approaches for comparison
- Console logging for behavior visualization
- Event listener setup and management

## 📚 Additional Resources

These examples provide a foundation for understanding performance optimization in JavaScript. Consider exploring:
- RequestAnimationFrame for animation throttling
- IntersectionObserver for scroll-based triggers
- Web Workers for heavy computation debouncing

---

**Note:** Open the browser console while interacting with the examples to see the debouncing and throttling effects in real-time!