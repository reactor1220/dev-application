# Fullstack Developer Hiring Test

Welcome! This is a technical assessment for candidates applying to join our team as a fullstack developer. It helps us understand how you work, think, and structure your code.

We're not looking for perfection. We're looking for clean thinking, good communication, and reliable execution.

---

## 👨‍💻 About the Role

We're building a small, remote team working on new projects in the **fitness and sports-tech industry**. This is a **new fullstack role** where you'll contribute across frontend and backend using **ReactJS, NextJS, and NodeJS**.

- This is a **remote contractor role**
- You'll work alongside a technical lead and other remote team members
- The role starts with a 3-month trial and may lead to ongoing work if it's a good fit
- You'll be responsible for your own hours, tools, and taxes

---

## 💰 Compensation

- **AUD $1,600 per month for full-time**, as a contractor  
- Part-time options are available depending on your experience and availability

---

## ✅ What You Need To Do

1. Complete the three coding tasks below
2. Push your work to your **own GitHub repository**
3. In the **root folder** of your repo, add a Markdown file with your CV:  
   `cv_{your-full-name}.md`
4. Submit your application using this form:  
   👉  https://forms.gle/3TpyZ8uHP3L9Nyq4A

> If your repo is private, make sure you grant us access to review it.

---

## 🧪 Task 1: Code Cleanup – "Fix This Component"

You've just joined the team and find the following component in production. Rewrite it to be clean and maintainable, keeping the exact same functionality.

```jsx
import React from "react";
export default function DataDisplay(props) {
  const [dt, setDt] = React.useState([]);
  React.useEffect(() => {
    fetch("https://jsonplaceholder.typicode.com/posts")
      .then((x) => x.json())
      .then((y) => {
        let z = [];
        for (let i = 0; i < y.length; i++) {
          if (i < 5) {
            z.push(y[i]);
          }
        }
        setDt(z);
      });
  }, []);
  return (
    <div>
      <h2>Stuff</h2>
      <ul>
        {dt.map((a) => (
          <li key={a.id}>{a.title}</li>
        ))}
      </ul>
    </div>
  );
}
```

**What we're looking for:**
- Clean, readable code structure
- Meaningful variable names
- Proper error handling
- Brief comments explaining your approach

---

## 📋 Task 2: Data List with Search

Build a React component that displays a list of users with search functionality.

**Requirements:**
- Use this sample data:
```javascript
const users = [
  { id: 1, name: 'John Smith', email: 'john@example.com', role: 'Developer' },
  { id: 2, name: 'Sarah Johnson', email: 'sarah@example.com', role: 'Designer' },
  { id: 3, name: 'Mike Wilson', email: 'mike@example.com', role: 'Manager' },
  { id: 4, name: 'Emma Davis', email: 'emma@example.com', role: 'Developer' },
  { id: 5, name: 'Tom Brown', email: 'tom@example.com', role: 'Designer' }
];
```
- Display all users in a clean list format
- Add a search input that filters users by name or email
- Show "No results found" when search returns no matches
- Clear, readable styling

**What we're looking for:**
- Component structure and state management
- Clean, reusable code organization
- User experience considerations

---

## ⏱ Task 3: Simple Countdown Timer

Build a React component that counts down from 10 to 0, updating once per second. When it reaches 0, display "Done!".

**Requirements:**
- Use React functional components and hooks
- No external libraries
- Include start/reset functionality
- Clean, readable code

**What we're looking for:**
- Understanding of React hooks (useState, useEffect)
- Proper cleanup of intervals/timers
- Simple, effective implementation

---

## 📝 Documentation Requirements

In your repository, include:

1. **README.md** – Brief explanation of your approach for each task
2. **cv_{your-full-name}.md** – Your CV in markdown format
3. **Comments in code** – Brief explanations where helpful

If you make any assumptions while completing a task, please note them clearly in your `README.md` under each task section.

We value clear communication and documentation skills highly.

---

## 🧠 What We're Really Looking For

- **Clean code organization** – How do you structure your files and components?
- **Problem-solving approach** – How do you break down requirements?
- **Communication skills** – Can you explain your decisions clearly?
- **Attention to detail** – Do you handle edge cases and follow instructions?
- **Remote work readiness** – Can you work independently and deliver quality results?

We care more about clarity and thoughtful structure than clever tricks or perfect styling.

---

## 📩 Final Step (Reminder)

Once you're done, make sure your GitHub repo includes:
- Your completed tasks
- A `cv_{your-full-name}.md` file in the root folder
- A brief `README.md` explaining your approach and assumptions

Then submit your repo link through this form:  
👉 https://forms.gle/3TpyZ8uHP3L9Nyq4A

If you run into any issues, feel free to leave a note in your form response.

---

**Good luck! We're excited to see your work.**
