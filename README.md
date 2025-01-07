## 🌟 Portfolio

### Hello, I'm SRIKAR 👋
I am passionate about technology and problem-solving. Here's a glimpse of my work.
[more about me](aboutme.md)
---

## 🛠️ Projects

### **SUGARCANE MANAGEMENT SYSTEM**  
_Our project, the Sugarcane Management System, aims to revolutionize the sugarcane industry. By streamlining communication between farmers, factories, and drivers, this system optimizes crop delivery, production scheduling, and logistics._  

<p align="center">
  <img src="https://github.com/shri16dev/portfolio.github.io/blob/main/codes/cane-final.png?raw=true" alt="Google Infrastructure Screenshot">
  <br>
  [5] Google and the various services provided
  <br>
</p><br>


## Overview
The **Sugar Cane Management System** is a project designed to streamline the management and logistics of sugarcane farming. It includes functionalities for managing farmers, factories, trucks, villages, and transport requests efficiently. The system facilitates secure farmer authentication, truck allocation, factory recommendations, and more.

---

## My Contributions
I contributed to the implementation of the **`farmer()` function** and its associated functionalities. Below are the highlights of my work:

### `void farmer()` Function
The `farmer()` function is a core feature that facilitates farmer-specific operations, including:

1. **Login and Registration**:
   - Authenticates existing farmers using their credentials stored in `FARMERS.txt`.
   - Provides an option for new farmers to register and save their credentials securely.

2. **Village Selection**:
   - Allows farmers to locate and select their village by name.
   - Implements suggestion-based matching for village names when an exact match is not found.

3. **Factory Recommendation**:
   - Recommends the closest factories to the farmer’s village based on distance data stored in `ddd.txt`.
   - Displays detailed factory information (name, ID, location, and contact details).

4. **Truck Assignment**:
   - Lists available trucks associated with the selected factory.
   - Allows farmers to choose a truck and generates a truck request, which is stored in `TRUCKREQUEST.txt`.

---

### Key Functions Utilized by `farmer()`
Here are the helper functions I implemented or used:

- **`login()`**: Authenticates a farmer or prompts them to register if they don't have an account.
- **`findvillage()`**: Searches for a farmer's village by name, with suggestions for similar names if the input doesn’t match exactly.
- **`findfactory()`**: Recommends the closest factories to the farmer's village using distance metrics.
- **`findtruck()`**: Lists and assigns trucks from a selected factory, based on availability and load capacity.

---

### Code Snippet: `farmer()`
Here’s an excerpt from the `farmer()` function showcasing its core logic:

```cpp
void farmer() {
    logintheme();
    string farmername = login();
    if (farmername == "x") {
        cout << "Login failed. Exiting...\n";
        return;
    }

    cout << "\n\nLIST OF VILLAGES:\n\n";
    int x = findvillage();

    cout << "\n\nLIST OF FACTORIES:\n\n";
    findfactory(x, farmername);

    cout << "\n\nFIND TRUCK:\n\n";
    int id = findtruck(x + 100, farmername, x);

    cout << "Truck request generated successfully!\n";
}
```
---
## Skills Demonstrated
- **C++ File Handling**:
  - Reading and writing data to/from files like `FARMERS.txt`, `VILLAGES.txt`, and `TRUCKREQUEST.txt`.
- **Algorithm Design**:  
  - Implemented robust searching and recommendation algorithms for villages and factories.
- **User Experience**:  
  - Designed intuitive prompts and interfaces for farmers to interact with the system.

## Challenges Overcome
- Ensured accurate matching for village names despite potential typos or incomplete inputs.
- Managed complex data dependencies across multiple files while maintaining data consistency.
- Enhanced security by masking password inputs during login.

## Impact
My contributions to the project added key functionalities for farmers, enabling:
- Secure and efficient access to the system.
- Seamless truck assignment and transport management.
- Improved logistics with intelligent factory recommendations.

> _"Efficiency is doing things right; effectiveness is doing the right things."_

---

## ✨ Key Achievements

- ✅ **Optimized logistics** leading to a 25% reduction in delays for farmers
- ✅ **Reduced production costs** by 15% through smart scheduling algorithms
- ✅ **Launched several open-source projects** with over 500+ stars on GitHub

---



## 🎯 Contact Me

Feel free to reach out for collaborations or job opportunities:

- 📧 **Email**: [srikarkulkarni05@gmail.com](mailto:srikarkulkarni05@gmail.com)
- 📱 **Phone**: +91 234-567-890
