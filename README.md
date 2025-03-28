# 🟢 **Automated Deadlock Detection Tool**

An advanced **Deadlock Detection Tool** that uses **Banker's Algorithm** to identify potential deadlocks in system processes. Built with **Python** and a user-friendly **Tkinter GUI**, this tool allows easy input of process data and provides real-time feedback on system safety.

---

## 📌 **Project Overview**
This project automates the detection of **deadlocks** in operating systems by analyzing **process dependencies** and **resource allocation**. It identifies **circular wait conditions** and suggests a safe execution sequence if no deadlock is present.

### ✅ **Key Objectives:**
- Detect **deadlocks** using Banker's Algorithm.
- Provide a **Graphical User Interface (GUI)** for easy input and visualization.
- Display the **Safe Sequence** if no deadlock is detected.
- **Auto-generate** a comprehensive project report in `.docx` format.

---

## 📂 **Project Structure**
Automated-Deadlock-Detection-Tool/ ├── main.py # Main script to launch the GUI ├── process.py # Process Management Module ├── res.py # Resource Management Module ├── banker.py # Banker's Algorithm Module ├── gui.py # Tkinter GUI Module ├── report_generator.py # Report Generation Module └── README.md # Project Documentation (this file)

markdown
Copy
Edit

---

## 📊 **Features**
- 🎨 **User-Friendly GUI**: Simple Tkinter interface for easy input and output.
- 🔍 **Deadlock Detection**: Identifies deadlocks in real-time using Banker's Algorithm.
- 📊 **Safe Sequence Display**: Outputs a safe sequence if no deadlock is found.
- 📄 **Report Generation**: Auto-creates a detailed `.docx` report of the analysis.
- 🛡️ **Error Handling**: Detects and manages invalid or inconsistent input.

---

## 🛠️ **Technologies Used**

### 💻 **Programming Language**
- Python 3.x

### 📚 **Libraries and Tools**
- **Tkinter**: For the graphical user interface.
- **python-docx**: For generating `.docx` reports.

### 🔧 **Other Tools**
- **GitHub**: For version control and collaboration.
- **Visual Studio Code**: For coding, debugging, and testing.

---

## 📐 **Module Breakdown**

1. **Process Management Module (`process.py`):**
   - Defines and manages process objects.
   - Stores the **allocated** and **maximum** resources for each process.

2. **Resource Manager Module (`res.py`):**
   - Handles **total resources** and keeps track of **available** resources.
   - Ensures real-time updates during execution.

3. **Banker's Algorithm Module (`banker.py`):**
   - Implements the **Banker's Algorithm** for deadlock detection.
   - Analyzes process requests and identifies **safe or unsafe** states.

4. **GUI Module (`gui.py`):**
   - **Tkinter-based** interface for user interaction.
   - Displays system status and **deadlock detection** results.

5. **Report Generator Module (`report_generator.py`):**
   - Generates a **.docx** report including:
      - Input details
      - Safe sequence (if available)
      - Deadlock status

---

## ▶️ **How to Run the Project**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Automated-Deadlock-Detection-Tool.git
   cd Automated-Deadlock-Detection-Tool
Install dependencies (if not already installed):

bash
Copy
Edit
pip install python-docx
Run the application:

bash
Copy
Edit
python main.py
📥 Input Format
Number of Processes (e.g., 5)

Maximum Resource Matrix (rows represent process maximum needs)

Current Allocation Matrix (rows represent allocated resources)

Available Resources (total available resources in the system)

Example Input:
less
Copy
Edit
Number of Processes: 5
Maximum Resources: [[7, 5, 3], [3, 2, 2], [9, 0, 2], [2, 2, 2], [4, 3, 3]]
Current Allocation: [[0, 1, 0], [2, 0, 0], [3, 0, 2], [2, 1, 1], [0, 0, 2]]
Available Resources: [3, 3, 2]
📊 Output Format
If the system is safe (no deadlock detected):

yaml
Copy
Edit
No Deadlock! Safe Sequence: [1, 3, 0, 2, 4]
If a deadlock is detected:

pgsql
Copy
Edit
Deadlock Detected! No safe sequence available.
📜 Flow Diagram
mathematica
Copy
Edit
Input Data ➜ Validate Input ➜ Apply Banker's Algorithm ➜
Check for Deadlock ➜ Display Result (Safe Sequence/Deadlock) ➜
Generate Report (Optional)
🔍 Sample Scenarios
Safe State (No Deadlock)
Input:

lua
Copy
Edit
Processes: 3
Max Resources: [[6, 3, 4], [3, 2, 2], [4, 3, 3]]
Allocated Resources: [[2, 1, 3], [1, 2, 1], [1, 0, 2]]
Available Resources: [3, 1, 2]
Output:

yaml
Copy
Edit
No Deadlock! Safe Sequence: [1, 0, 2]
Deadlock Detected
Input:

lua
Copy
Edit
Processes: 3
Max Resources: [[4, 3, 2], [2, 1, 3], [3, 2, 2]]
Allocated Resources: [[2, 2, 1], [2, 0, 2], [1, 1, 1]]
Available Resources: [0, 0, 0]
Output:

pgsql
Copy
Edit
Deadlock Detected! No safe sequence available.
📈 Future Scope
🌐 Web Interface using Flask/Django for accessibility.

🔀 Implementing Multi-threading for faster deadlock detection.

📊 Real-Time Monitoring for dynamic process management.

📥 Data Import/Export support for CSV and Excel.

📖 Revision Tracking
Repository Name: Automated-Deadlock-Detection-Tool

GitHub Link: [Insert GitHub Link Here]

📚 References
Operating System Concepts – Silberschatz, Galvin, Gagne

Python Documentation – docs.python.org

Banker's Algorithm – System Safety Analysis

📧 Contact
For any questions or contributions:

📧 Email: yourname@example.com

🔗 GitHub: yourusername

📜 License
This project is licensed under the MIT License.

