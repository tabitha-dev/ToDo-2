# 📝 Todo App – A Vue.js Project

An interactive **Todo App** designed with Vue.js and styled beautifully with responsive CSS. This app showcases essential web development skills such as **state management**, **local storage integration**, and **dynamic user interactions**. Customize your tasks and enjoy an intuitive interface!

---

## 🌟 Key Features

- **📋 Add Tasks:** Add new tasks to your todo list with ease.  
- **✔️ Mark as Complete:** Track your progress by marking tasks as done.  
- **🚮 Delete Tasks:** Remove completed or unnecessary tasks.  
- **🗂️ Show/Hide Completed Tasks:** Toggle visibility of completed tasks.  
- **📊 Completion Progress:** See a percentage breakdown of completed tasks.  
- **🎨 Customizable Backgrounds:** Choose from a variety of stunning backgrounds.  
- **💾 Persistent Storage:** Saves your tasks locally so your list is preserved even after refreshing.  

---

## 📖 How to Use

1. **Add Tasks:**  
   Type your task into the input field and click the **`+`** button or press **Enter**.  

2. **Mark Complete:**  
   Check the box next to a task to mark it as complete.  

3. **Show/Hide Completed Tasks:**  
   Click the **`Show Complete`** or **`Hide Complete`** button to toggle visibility of completed tasks.  

4. **Delete Tasks:**  
   Hover over a task and click the trash icon to delete it.  

5. **Change Backgrounds:**  
   Use the dropdown menu to select a new background image for the app.  

6. **Clear All Tasks:**  
   Click the **`Clear All`** button to reset the list.  

---

## 🔥 Enhancements

Take the app to the next level with these ideas:

- **🗂️ Categories:** Add tags or categories to organize tasks.  
- **📆 Due Dates:** Integrate due dates and reminders.  
- **🔔 Notifications:** Push notifications for pending tasks.  
- **🌎 Online Syncing:** Enable syncing across devices using an online backend.  
- **🎨 Dark Mode:** Add a toggle for dark and light themes.  

---

## 🖥️ Code Structure Overview

### **HTML**
- Semantic structure for the todo list and controls.
- Dropdown menu for selecting background images.
- Footer with social links and credits.

### **CSS**
- Responsive, modern design with clean typography and subtle animations.
- Hover and transition effects for interactivity.
- Customizable styles for buttons, inputs, and todo items.

### **Vue.js Functionality**
- **`data()`**: Stores the todo list, background selection, and input state.
- **Computed Properties**: Calculates pending/completed tasks and displays today's date.
- **Local Storage**: Saves tasks locally to maintain state after a refresh.
- **Methods**: Handles core features like adding, deleting, toggling tasks, and clearing the list.
- **Lifecycle Hooks**: Initializes background image and retrieves stored tasks on load.

---

## 📋 Code Highlights

### Add New Todo:
```javascript
addItem() {
  if (this.new_todo) {
    this.todoList.unshift({
      id: this.todoList.length,
      title: this.new_todo,
      done: false,
    });
  }
  this.new_todo = '';
}
---
## 🌈 Dynamic Background Change
setBackground() {
  document.body.style.backgroundImage = `url(${this.background})`;
}
---
## 🔄 Toggle Completed Tasks Visibility
toggleShowComplete() {
  this.showComplete = !this.showComplete;
}
---
## 🌐 Social Links
Designed and developed by Tabitha-Dev. Connect with me:

LinkedIn
GitHub
CodePen
Replit

---
📄 License
This project is open-source and licensed under the MIT License. Feel free to modify and share.
---
💡 Inspirational Quote
"Believe you can and you're halfway there." – Theodore Roosevelt

🚀 Try the App and Boost Your Productivity!
