# Linux & Git Command Reference

## 1. Basic Linux Commands
```bash
pwd                     # Print working directory
ls                      # List files
ls -la                  # List files (detailed + hidden)
ls -s                   # Show file sizes
clear                   # Clear terminal
whoami                  # Show current logged in user
2. File & Directory Management
bash
Copy code
cd /path/to/dir         # Change directory
cd ~                    # Go to home directory
cd ..                   # Move one level up
mkdir devops            # Create directory
mkdir -p devops         # Create directory (no error if exists)
touch hello.txt         # Create empty file
echo "This is text" > hello.txt   # Write text to file (overwrite)
cat hello.txt           # Show file contents
vim hello.txt           # Edit file in vim
rm file.txt             # Delete file
3. Package Management (Ubuntu/Debian)
bash
Copy code
sudo apt update                 # Update package index
sudo apt install -y nginx       # Install nginx
sudo systemctl restart nginx    # Restart nginx service
sudo systemctl status nginx     # Check nginx status
4. SSH & Keys
bash
Copy code
chmod 400 Batch8key.pem
ssh -i "Batch8key.pem" ubuntu@ec2-34-233-133-153.compute-1.amazonaws.com
5. Git Basics
bash
Copy code
git init                        # Initialize repository
git status                      # Check repo status
git add file.txt                # Stage file
git add .                       # Stage all files
git commit -m "message"         # Commit changes
git log                         # Show commit history
git branch                      # List branches
git checkout -b dev             # Create & switch to 'dev' branch
git checkout master             # Switch back to master
git merge dev                   # Merge dev into master
6. Git File Operations
bash
Copy code
git rm --cached file.txt        # Remove file from git tracking (keep locally)
git restore file.txt            # Restore deleted/modified file
rm file.txt                     # Delete file locally
7. Example Workflow
bash
Copy code
# Create project folder
mkdir git-for-devops && cd git-for-devops

# Initialize git
git init

# Create and commit files
touch nibba.txt nibbi.txt
git add nibba.txt nibbi.txt
git commit -m "Added nibba and nibbi"

# Create feature branch
git checkout -b dev
touch nibbu.txt
git add nibbu.txt
git commit -m "Added nibbu"

# Merge into master
git checkout master
git merge dev
yaml
Copy code

---




