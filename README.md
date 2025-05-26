## Experiment 2: Welcome Message in Message Box with IF Condition and Switch Case

### Aim
To display a customized welcome message using Message Box activity, along with If and Switch Case control structures in UiPath.

### Materials Required
- UiPath Studio
- Windows OS

### Procedure
1. Open UiPath Studio and create a new Process project.
2. Name the project (e.g., `WelcomeMessageSwitchCase`) and click "Create".
3. Open `Main.xaml` and perform the following steps:

#### Using If Condition:
4. Drag an **Input Dialog** activity to ask the user to enter their name.
5. Store the result in a variable, e.g., `userName`.
6. Add an **If** activity to check if `userName = "Admin"`.
   - In the **Then** branch, use a **Message Box** to display `"Welcome Admin!"`.
   - In the **Else** branch, display `"Welcome User!"`.

#### Using Switch Case:
7. Drag another **Input Dialog** to ask for a role (e.g., Admin, Manager, Guest).
8. Store the result in a variable, e.g., `userRole`.
9. Add a **Switch** activity with `userRole` as the expression and type as `String`.
10. Add cases for:
    - `"Admin"` → Message Box: `"Access granted to Admin Portal."`
    - `"Manager"` → Message Box: `"Access granted to Management Dashboard."`
    - `"Guest"` → Message Box: `"Limited access granted."`
    - **Default** → Message Box: `"Role not recognized."`

11. Run the workflow.

### Output

![Screenshot 2025-05-05 092344](https://github.com/user-attachments/assets/13b5ba36-89df-49ec-afa3-d4f57028dd5f)

![Screenshot 2025-05-05 092413](https://github.com/user-attachments/assets/d604f2ca-6b7c-43df-8dda-e4ccc86654a3)

![Screenshot 2025-05-05 092427](https://github.com/user-attachments/assets/e77da35c-de35-4f84-897f-5aba99795ad8)

![Screenshot 2025-05-05 092438](https://github.com/user-attachments/assets/f73b8872-3d3c-47af-bd3d-d742ca9c694e)

### Result
The workflow displays different welcome messages based on user input using If and Switch Case conditions.

