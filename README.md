

## 📁 **Interactive File/Folder Explorer**

A **recursive tree-view component** that displays a hierarchical file and folder structure with interactive features.

### **Key Features:**

#### 1. **Visual Hierarchy**
- 📂 **Folders**: Display with expandable/collapsible icons
- 📄 **Files**: Display with static file icons
- **Nested Structure**: Unlimited depth - folders can contain folders and files

#### 2. **Interactive Elements**
- **Click to Expand/Collapse**: Click folder icon to toggle visibility of children
- **Visual Feedback**: 
  - 📂 **Closed folder icon** when collapsed
  - 📁 **Open folder icon** when expanded

#### 3. **CRUD Operations**
- **➕ Add Button**: Creates new sub-folders inside any folder
  - Generates random ID and name
  - New items are folders by default
- **➖ Remove Button**: Deletes folders/files at any level
  - Recursively searches and removes from entire tree

#### 4. **Technical Implementation**
- **Recursive Rendering**: Each folder can contain more `List` components
- **State Management**: 
  - Global state for entire tree structure
  - Local state for expand/collapse per folder
- **Immutable Updates**: Uses pure functions to update nested data

---

### **Use Cases:**
✅ File system explorers  
✅ Project directory viewers  
✅ Document management systems  
✅ Navigation menus  
✅ Category/subcategory organizers  

---

### **Example Structure:**
```
📁 Root Folder (expandable)
  ├── 📄 file1.txt
  ├── 📁 Subfolder 1 (expandable)
  │   ├── 📄 file2.txt
  │   └── 📁 Nested Folder
  │       └── 📄 file3.txt
  └── 📁 Subfolder 2
      └── 📄 file4.txt
```

Each folder has **+** and **-** buttons to add/remove items dynamically! 🎯
