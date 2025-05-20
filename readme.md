#  Jenkins CI/CD Pipeline for Streamlit App




###  GitHub Integration

- I connected my GitHub repository under:
  **Jenkins > Pipeline > Definition > Pipeline script from SCM**
- I selected the correct GitHub repository and set the branch to `main`
- Applied the changes and saved the configuration
![Initial Failure](https://github.com/user-attachments/assets/1bada160-11a5-4ab9-9b9e-6f52e68991e1)



---

###  Initial Pipeline Failure

- The pipeline failed at first because Python was not installed in the Jenkins environment
- I also forgot to create a virtual environment before trying to install dependencies
![SCM Configuration](https://github.com/user-attachments/assets/232f9257-7475-4cd6-973d-4f74257e2728)

---

###  Fix Applied

- Installed Python inside the Jenkins container
- Created a virtual environment as part of the pipeline steps

---

###  Pipeline Successful

- After resolving the above issues, the pipeline ran successfully

![Pipeline Flow](https://github.com/user-attachments/assets/ac10d5ca-a01d-4f3b-9e64-92dbf07b3948)

---

###  Final Output

- This is the final output from the Jenkins console, showing a successful build

![Console Output](https://github.com/user-attachments/assets/689b964c-141d-490c-b753-42cc8028aa50)

---


