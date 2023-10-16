# form-html-css
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Employee Details</title>
</head>
<body>
    <div class="left-section">
        <!-- Content for the left section goes here -->
        <form>
            <h2>Employee </h2>
            <label for="employeeId">Employee ID </label>  
            <br>
            <label for="nic">NIC </label>
            <br>
            <label for="title">Title </label> 
            <br><br>
            <label for="firstName">First Name</label>
            <br>
            <label for="lastName">Last Name</label> 
            <br>
            <label for="gender">Gender</label> 
            <br>
            <label for="dob">Date of Birth</label> 
            <br>
            <label for="age">Age</label>
            <br>
            <label for="salary">Salary</label>

        </form>
       
    </div>
    <div class="right-section">
        <!-- Content for the right section goes here -->
        <form>
            <h2>Details</h2>
        
            <input type="text" id="employeeId" name="employeeId" required>
            <br>
            <input type="text" id="nic" name="nic" required>
            <br>
            <select id="title" name="title">
                <option value="Mr">Mr</option>
                <option value="Ms">Ms</option>
                <option value="Mrs">Mrs</option>
            </select><br>
            <input type="text" id="firstName" name="firstName">
            <br>
            <input type="text" id="lastName" name="lastName">
            <br>
            <input type="text" id="gender" name="gender">
            <br>
            <input type="text" id="dob" name="dob">
            <br>
            <input type="text" id="age" name="age">
            <br>
            <input type="text" id="salary" name="salary">
            <br><br>
            <input type="reset" value="Cancel"> &nbsp;&nbsp;<input type="submit" value="Submit">


        </form>
        <script>
            // JavaScript code to display gender based on selected title
            const titleSelect = document.getElementById("title");
            const genderInput = document.getElementById("gender");
    
            titleSelect.addEventListener("change", () => {
                const selectedTitle = titleSelect.value;
                let gender = "";
    
                switch (selectedTitle) {
                    case "Mr":
                        gender = "Male";
                        break;
                    case "Ms":
                    case "Mrs":
                        gender = "Female";
                        break;
                    default:
                        gender = "";
                }
    
                genderInput.value = gender;
            });
        </script>
    </div>
</body>
</html>
