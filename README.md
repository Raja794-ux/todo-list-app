# To-Do List Application

A modern, feature-rich to-do list application with local storage functionality. Built with vanilla HTML, CSS, and JavaScript.

## Features

✨ **Core Features:**
- ✅ Add new tasks
- 🗑️ Delete tasks
- ☑️ Mark tasks as completed
- 💾 Persistent storage using browser's Local Storage
- 🎨 Beautiful, responsive UI
- 📊 Task statistics (Total & Completed count)

🔧 **Advanced Features:**
- 🔍 Filter tasks (All, Active, Completed)
- 🧹 Clear all completed tasks at once
- ⌨️ Enter key support for adding tasks
- 📱 Fully responsive design (mobile, tablet, desktop)
- ✨ Smooth animations and transitions
- 🛡️ XSS protection (HTML escaping)

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No server or build tools required!

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Raja794-ux/todo-list-app.git
cd todo-list-app
```

2. Open `index.html` in your browser:
   - Double-click the `index.html` file, or
   - Right-click and select "Open with" your preferred browser

### Or Use Live Server (Optional)
For a better development experience, use VS Code's Live Server extension:

1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"
4. The app will open at `http://localhost:5500`

## Usage

### Adding Tasks
1. Type your task in the input field
2. Click "Add Task" or press Enter
3. Task will be added to the list

### Managing Tasks
- **Mark Complete**: Click the checkbox next to a task
- **Delete**: Click the "Delete" button on a task
- **Filter**: Use the filter buttons (All, Active, Completed) to view specific tasks
- **Clear Completed**: Click "Clear Completed" to remove all finished tasks

### Data Persistence
- All tasks are automatically saved to your browser's Local Storage
- Your tasks will persist even after closing and reopening the browser
- Data is stored locally on your device (not on any server)

## Project Structure

```
todo-list-app/
├── index.html       # HTML structure
├── styles.css       # Styling and responsive design
├── script.js        # JavaScript functionality
└── README.md        # Documentation
```

## File Descriptions

### `index.html`
- Main HTML structure
- Input section for adding tasks
- Filter buttons
- Statistics display
- Todo list container

### `styles.css`
- Modern gradient design
- Responsive grid and flexbox layouts
- Smooth animations and transitions
- Mobile-first responsive design
- Custom scrollbar styling

### `script.js`
- Task management logic (add, delete, toggle)
- Local storage integration
- Filtering functionality
- DOM manipulation
- Event handling

## Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | Latest | ✅ Fully supported |
| Firefox | Latest | ✅ Fully supported |
| Safari | Latest | ✅ Fully supported |
| Edge | Latest | ✅ Fully supported |
| IE 11 | - | ❌ Not supported |

## Local Storage Details

The app uses the browser's `localStorage` API to persist data:

- **Key**: `todos`
- **Format**: JSON array of todo objects
- **Storage Limit**: ~5-10 MB (varies by browser)
- **Persistence**: Data persists until manually cleared

### Local Storage Structure
```javascript
[
  {
    id: 1234567890,
    text: "Buy groceries",
    completed: false,
    createdAt: "9/6/2026, 10:30:45 AM"
  },
  // ... more todos
]
```

### Clear Local Storage
To clear all stored tasks (via browser console):
```javascript
localStorage.removeItem('todos');
```

## Future Enhancements

- 🌙 Dark mode toggle
- 📅 Due dates and reminders
- 🏷️ Task categories/tags
- 🔄 Drag and drop to reorder
- 📤 Export/Import functionality
- ☁️ Cloud sync with Firebase/Supabase
- 🔔 Notifications
- 🎨 Customizable themes

## Security Notes

- ✅ XSS protection: HTML is escaped before rendering
- ✅ No sensitive data collected
- ✅ Data stored locally only
- ✅ No external API calls
- ✅ No tracking or analytics

## Performance

- ⚡ Lightweight (~5KB total)
- ⚡ Zero dependencies
- ⚡ Instant load time
- ⚡ Smooth 60fps animations

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests
- Improve documentation

## License

This project is open source and available under the MIT License.

## Support

Have questions or issues? 
- Check the GitHub Issues page
- Review the source code with inline comments
- Consult the documentation

## Author

Created with ❤️ by Raja794-ux

---

**Happy task managing! 🚀**
