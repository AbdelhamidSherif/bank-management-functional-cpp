# Bank Client Management System

A comprehensive C++ console application for managing bank client records with full CRUD (Create, Read, Update, Delete) operations.

## 🏦 Overview

This Bank Client Management System is a console-based application written in C++ that demonstrates **Functional Programming** principles for managing bank client accounts. The system uses file-based storage to persist client data and provides a user-friendly menu-driven interface.

### 🎯 Programming Paradigm

This version of the system is built using **Functional Programming** approach, featuring:
- **Function-based architecture** with clear separation of concerns
- **Pure functions** for data transformation and validation
- **Stateless operations** with data passed between functions
- **Procedural flow** with structured programming techniques

### 🔄 Future Development

An **Object-Oriented Programming (OOP)** version of this system is planned for development, which will include:
- **Class-based design** with proper encapsulation
- **Inheritance hierarchies** for different account types
- **Polymorphism** for flexible client management
- **Design patterns** implementation (Factory, Observer, etc.)
- **Better code reusability** and maintainability

This functional version serves as a foundation and reference point for comparing programming paradigms and understanding the evolution from procedural to object-oriented design.

## ✨ Features

- **Client List Display**: View all registered clients with their details in a formatted table
- **Add New Clients**: Register new clients with validation for duplicate account numbers
- **Delete Clients**: Remove client records with confirmation prompts
- **Update Client Info**: Modify existing client information
- **Find Clients**: Search for specific clients by account number
- **File-Based Storage**: All data is persisted in a text file (`Clients.txt`)
- **Data Validation**: Ensures unique account numbers and proper data formatting

## 🗂️ Data Structure

Each client record contains:
- **Account Number**: Unique identifier for each client
- **PIN Code**: Client's personal identification number
- **Name**: Full name of the client
- **Phone**: Contact phone number
- **Account Balance**: Current balance in the account

## 🚀 Getting Started

### Prerequisites

- C++ compiler (GCC, MSVC, or Clang)
- Standard C++ libraries
- Windows OS (due to `system("cls")` and `system("pause>0")` commands)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/AbdelhamidSherif/bank-client-management.git
   cd bank-client-management
   ```

2. **Compile the program**
   ```bash
   g++ -o bank_system main.cpp
   ```

3. **Run the application**
   ```bash
   ./bank_system
   ```

## 📋 Usage

### Main Menu Options

When you run the program, you'll see a main menu with the following options:

1. **Show Client List** - Displays all clients in a formatted table
2. **Add New Client** - Add one or more new clients to the system
3. **Delete Client** - Remove a client by account number
4. **Update Client Info** - Modify existing client information
5. **Find Client** - Search for a client by account number
6. **Exit** - Close the application

### Adding a New Client

```
Enter Account Number? A101
Enter PinCode? 1234
Enter Name? John Doe
Enter Phone? +1234567890
Enter AccountBalance? 5000.00
```

### Sample Data Format

The system stores data in `Clients.txt` with the following format:
```
A101#//#1234#//#John Doe#//#+1234567890#//#5000.00
A102#//#5678#//#Jane Smith#//#+0987654321#//#7500.50
```

## 🏗️ Code Structure

### Core Functions

- `ShowMainMenue()` - Displays the main menu and handles user navigation
- `LoadCleintsDataFromFile()` - Reads client data from file into memory
- `SaveCleintsDataToFile()` - Writes client data from memory to file
- `ConvertLinetoRecord()` - Converts file line to client structure
- `ConvertRecordToLine()` - Converts client structure to file line
- `FindClientByAccountNumber()` - Searches for a client by account number

### Key Classes/Structures

```cpp
struct sClient {
    string AccountNumber;
    string PinCode;
    string Name;
    string Phone;
    double AccountBalance;
    bool MarkForDelete;
};
```

## 📁 File Structure

```
bank-client-management/
│
├── main.cpp           # Main source code file
├── Clients.txt        # Client data storage (auto-generated)
├── README.md          # This file
└── .gitignore         # Git ignore file
```

## 🔒 Security Features

- **Account Number Validation**: Prevents duplicate account numbers
- **Confirmation Prompts**: Requires confirmation before deleting or updating records
- **Data Integrity**: Uses structured file format to maintain data consistency

## 🛠️ Future Enhancements

- [ ] Add password protection for system access
- [ ] Implement data encryption for sensitive information
- [ ] Add transaction history tracking
- [ ] Create a GUI version using Qt or similar framework
- [ ] Add database support (MySQL/SQLite)
- [ ] Implement user roles and permissions
- [ ] Add data backup and restore functionality
- [ ] Include data export options (CSV, PDF)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Steps to Contribute

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Abdelhamid Sherif**
- GitHub: [@AbdelhamidSherif](https://github.com/AbdelhamidSherif)
- LinkedIn: [abdelhamid-sherif](https://linkedin.com/in/abdelhamid-sherif)

## 📞 Support

If you have any questions or need help with the system, please:
1. Check the existing issues in the repository
2. Create a new issue with a detailed description
3. Contact the maintainer directly

## 🙏 Acknowledgments

- Thanks to all contributors who have helped improve this project
- Inspired by real-world banking systems and best practices in C++ development

---

⭐ If you found this project helpful, please give it a star on GitHub!
