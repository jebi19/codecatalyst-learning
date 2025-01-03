# Code Catalyst
 
Hostel Attendence System

# GIT
Git is a distributed version control system (DVCS) that allows developers to track changes in their codebase, collaborate with others, and manage different versions of their projects efficiently.

### **Why use git?**

1. Version Control: Git helps in tracking changes, allowing you to revert to previous states if something goes wrong.
2. Collaboration: It enables multiple developers to work on a project simultaneously without interfering with each other’s work.
3. Backup: Your entire project history is saved in a Git repository, providing a backup of all versions.
4. Branching and Merging: Git’s branching model allows you to experiment with new features or bug fixes independently from the main project.
5. Open Source Projects: Most open source projects use Git for version control. Learning Git allows you to contribute to these projects.
6. Industry Standard: Git is widely used in the software industry, making it an essential skill for developers.

### **1. Configure Git Bash**  
Set up Git with your GitHub account: 

1. git config --global user.name "Your GitHub Name"  

2. git config --global user.email "your.github.email@example.com"  
     
### **2. Create a Repository**  
1. Create a repository in VS Code:    
   mkdir codecatalyst-learning  
   cd codecatalyst-learning  
   git init  
 
### **3. Push the Repository to GitHub**  
1. Connect your local repository to a remote repository on GitHub:  
   
   git remote add origin (repository-URL)  
   git push origin main  
     
### **4. Add a Sample File**  
1. Add a `README.md` file and stage it:  
   
   echo "readme file" > README.md  
   git add README.md  
   git commit -m "Initial commit"  
     
### **5. Make Changes and View Staged Changes**  
1. Edit the `README.md` file and check the status:  
   
   git status  
     
### **6. Commit Changes**  
1. Commit your changes with a meaningful message:  
   
   git commit -m "Newly committed change"  
     
### **7. Push Changes to GitHub**  
1. Push the committed changes to your remote repository:  
   
   git push origin main  

### **8. Create a New Branch**  
1. Create a branch named `secondary-branch`:  
   
   git branch secondary-branch  

### **9. Switch to the New Branch**  
1. Switch to the `secondary-branch` and push it to GitHub:  
   
   git checkout secondary-branch  
   git add .  
   git commit -m "New branch"  
   git push origin secondary-branch  

### **10. Merge Branches**  
1. Merge the `secondary-branch` into the `main` branch:  
   
   git checkout main  
   git pull origin main  
   git merge secondary-branch  

### **11. Simulate and Resolve Merge Conflicts**  
1. Edit the same file in both `main` and `secondary-branch` to create a conflict.  
2. When merging, resolve the conflict:  
   - Remove conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) in the file.  
   - Stage and commit the resolved file:  
     
     git add README.md  
     git commit -m "Resolved merge conflict in README.md"    
     git push origin main  

### **12. Confirm the Merge**  
 git log --oneline --graph  
  