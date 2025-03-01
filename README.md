# LINUX SHELL SCRIPTING
# Table of Contents

1. **Project Overview**
2. **Project Steps and Commands**
   - 2.1 [Create Project Directory]
     <img width="529" alt="Snipaste_2025-03-01_19-58-57" src="https://github.com/user-attachments/assets/2471c150-e12e-4c94-87f7-af943e0320a6" />

   - 2.2 [Initialize Git Repository]
     <img width="540" alt="Snipaste_2025-03-01_19-59-20" src="https://github.com/user-attachments/assets/03de63e3-3bdb-400b-bb48-8b5b6c323182" />

   - 2.3 [Create the Bash Script File (.sh)]
     <img width="493" alt="Snipaste_2025-03-01_19-59-51" src="https://github.com/user-attachments/assets/ff532589-712d-42e3-a0fa-69190ad133f6" />

     -2.3 [Enter your bash code]
     ![image](https://github.com/user-attachments/assets/79b0d3d2-5632-43af-b0ec-07e7373adfc7)


   - 2.4 [Make the Script Executable]
   ![image](https://github.com/user-attachments/assets/b7f48060-2040-45b3-bec9-09ec99d43e26)

3. **Script Implementation Steps**
   - 3.1 [Prompt for User Input]!
   -![image](https://github.com/user-attachments/assets/b033e9cf-facb-400b-b21a-11d9cea2094a)

   - ![image](https://github.com/user-attachments/assets/dfc93bb5-162b-4842-9018-60f5922f5408)


   - 3.2 [Ask for Table Type (Full or Partial)]
   - ![image](https://github.com/user-attachments/assets/647a381b-14c1-4b26-9039-7dc0697a8188)
   - ![image](https://github.com/user-attachments/assets/05a87cd3-530a-495a-a0ab-21b95861b825)


   - 3.3 [Full Multiplication Table]
   - ![image](https://github.com/user-attachments/assets/1d712192-99b5-434a-86de-f4f39ea18a66)

   - 3.4 [Partial Multiplication Table]
   - ![image](https://github.com/user-attachments/assets/7bed7ca8-a9ed-4433-b4b0-98ec559cbabc)

   - 3.5 [Validate Input Range for Partial Table]
   - ![image](https://github.com/user-attachments/assets/b6eed785-4055-4600-b214-41952aa5c3e9)

   - 3.6 [Handle Invalid Options]
   - ![image](https://github.com/user-attachments/assets/421ce0cf-7e71-4acc-959a-26f203fcd0b7)
   - ![image](https://github.com/user-attachments/assets/cd0122a3-1ed3-4c8a-86cb-ad5c0e7e87da)


## 4. Troubleshooting (Common Issues and Solutions)
### 4.1. Script Permission Denied
    - If you encounter a “Permission Denied” error when running the script, ensure the script has executable permissions.
    - Solution: Run chmod +x multiplication_table.sh to make the script executable.
### 4.2. Invalid Input for Number
    - If the user enters a non-numeric value, the script may behave unexpectedly as it expects a number for multiplication.
    - Solution: Add input validation to ensure that only numbers are accepted. For example:

    ```sh 
    if ! [[ "$number" =~ ^[0-9]+$ ]]; then
    echo "Invalid input. Please enter a valid number."
    exit 1
    fi
    ```

### 4.3. Invalid Range in Partial Table
    - If the user inputs a start number greater than the end number, the script will display an "Invalid range" error.
    - Solution: Make sure the start number is less than or equal to the end number, as shown in the range validation code.

### 4.4. Git Remote Connection Issues
    - If you have trouble pushing code to the GitHub repository, verify that the remote URL is correct and that you have the necessary permissions.
    - Solution: Run git remote -v to check the remote URL and verify access. If there are issues, re-add the remote with the correct URL using git remote add origin <repository_url>.
