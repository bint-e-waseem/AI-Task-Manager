# AI-Task-Manager
# 🧠 AI Agent Task Management System

A comprehensive Object-Oriented Programming (OOP) based task management system built in Python for managing multiple AI agents and their assigned tasks.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🌟 Overview

The **AI Agent Task Management System** is a Python application that demonstrates Object-Oriented Programming principles through a practical task management solution. It allows users to create and manage multiple AI agents, assign tasks to them, and persist data using file handling.

This project was developed as part of an AI/ML coursework to showcase:
- **OOP Principles**: Encapsulation, Inheritance, and Polymorphism
- **File Handling**: Data persistence with text files
- **User Interaction**: Command-line interface with menu-driven navigation
- **Real-world Application**: Task management for AI agent systems

## ✨ Features

### Core Features
- **Agent Management**: Create and manage multiple AI agents with names and roles
- **Task Assignment**: Assign tasks to specific agents
- **Task Display**: View all tasks assigned to an agent or all agents
- **Status Tracking**: Track agent status (Active/Inactive)
- **Summary Reports**: Generate comprehensive summaries of all agents and their tasks

### Bonus Features 🌟
- **Persistent Storage**: Save tasks to a text file (`tasks_data.txt`)
- **Auto-Load**: Automatically load saved tasks when the system starts
- **Error Handling**: Robust error handling for file operations

## 🚀 Installation

### Prerequisites
- Python 3.6 or higher
- No additional libraries required (uses only built-in modules)

### Clone the Repository
```bash
git clone https://github.com/yourusername/ai-agent-task-manager.git
cd ai-agent-task-manager
```

### Run the Application
```bash
python agent_task_manager.py
```

## 💻 Usage

### Interactive Menu System

The application provides a user-friendly menu with the following options:

```
--------------------------------------------------
MAIN MENU
--------------------------------------------------
1. Add a new agent
2. Assign task to an agent
3. Display all agents and their tasks
4. Display specific agent's tasks
5. Save tasks to file (BONUS)
6. Load tasks from file (BONUS)
7. Exit
--------------------------------------------------
```

### Quick Start Guide

#### 1. Adding an Agent
```bash
Enter your choice (1-7): 1
Enter agent name: DataProcessor
Enter agent role: Data Analyst
Agent DataProcessor added successfully!
```

#### 2. Assigning a Task
```bash
Enter your choice (1-7): 2
Available agents:
1. DataProcessor (Data Analyst)
Select agent (number): 1
Enter task description: Process customer data for Q4
Task 'Process customer data for Q4' assigned to DataProcessor.
```

#### 3. Viewing All Agents
```bash
Enter your choice (1-7): 3

============================================================
AGENT TASK MANAGEMENT SYSTEM - SUMMARY
============================================================
Agent: DataProcessor | Role: Data Analyst | Status: Active | Tasks: 1
--- Tasks for DataProcessor (Data Analyst) ---
1. Process customer data for Q4
--------------------------------------------------
Total Agents: 1
Total Tasks: 1
============================================================
```

#### 4. Saving Tasks to File
```bash
Enter your choice (1-7): 5
Tasks successfully saved to tasks_data.txt!
```

## 🏗️ Code Structure

### Class Architecture

```
┌─────────────────────┐
│      Agent          │
├─────────────────────┤
│ - name: str         │
│ - role: str         │
│ - status: str       │
│ - tasks: list       │
├─────────────────────┤
│ + __init__()        │
│ + assign_task()     │
│ + display_tasks()   │
│ + get_summary()     │
└─────────────────────┘
         │
         │ uses
         ▼
┌─────────────────────┐
│   AgentManager      │
├─────────────────────┤
│ - agents: list      │
│ - filename: str     │
├─────────────────────┤
│ + add_agent()       │
│ + display_all()     │
│ + save_tasks()      │
│ + load_tasks()      │
└─────────────────────┘
```

### Key Methods

#### Agent Class
| Method | Description |
|--------|-------------|
| `__init__(name, role)` | Constructor initializing agent attributes |
| `assign_task(task)` | Adds a new task to the agent's task list |
| `display_tasks()` | Prints all tasks assigned to the agent |
| `get_summary()` | Returns a formatted summary of the agent |

#### AgentManager Class
| Method | Description |
|--------|-------------|
| `add_agent(agent)` | Adds a new agent to the system |
| `display_all_agents()` | Shows a summary of all agents and their tasks |
| `save_tasks_to_file()` | Persists all agent data to a text file |
| `load_tasks_from_file()` | Loads agent data from a text file |

## 📁 File Structure

```
ai-agent-task-manager/
│
├── agent_task_manager.py    # Main application file
├── tasks_data.txt           # Persistence file (auto-generated)
├── README.md                # Project documentation
└── requirements.txt         # Project dependencies (none required)
```

## 🎯 Learning Outcomes

Through this project, I demonstrated:

1. **Object-Oriented Programming**
   - Class design and instantiation
   - Encapsulation with private attributes
   - Method definitions and usage

2. **File Handling**
   - Reading from and writing to text files
   - Data serialization and deserialization
   - Exception handling for file operations

3. **Software Design Patterns**
   - Manager pattern for handling collections
   - Menu-driven architecture for user interaction

4. **Practical Application**
   - Real-world task management
   - Multi-agent system simulation
   - Data persistence strategies

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Suggested Improvements
- [ ] Add priority levels to tasks
- [ ] Implement task deadlines
- [ ] Create GUI interface
- [ ] Add database support (SQLite)
- [ ] Implement task statuses (Pending, In Progress, Complete)
- [ ] Add agent collaboration features

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📫 Contact

**Yashfa waseem** : yashfawaseem2006@gmail.com

**Project Link**: [https://github.com/yourusername/ai-agent-task-manager](https://github.com/yourusername/ai-agent-task-manager)

---

##  Acknowledgments

- Course instructor for inspiring this project
- Python community for excellent documentation
- Open source contributors for their continuous support

---

### ⭐ Support This Project

If you found this project helpful, please give it a star on GitHub! Your support motivates me to create more educational content.

[![GitHub Stars](https://img.shields.io/github/stars/yourusername/ai-agent-task-manager?style=social)](https://github.com/yourusername/ai-agent-task-manager)

**Happy Coding! 🚀**
