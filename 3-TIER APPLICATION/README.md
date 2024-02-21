
# 3-TIER APPLICATION

To develop an application which includes presentation layer, logic layer and database layer.


## Theory
 In a three-tier architecture with Python Tkinter as the front end and MySQL as the backend, the 
application is divided into three logical components: presentation, logic or application, and data 
storage. 

**1.Presentation Tier (Front End - Python Tkinter):** 
  - Responsible for user interface and user interaction. 
  - Utilizes Python Tkinter for GUI development, creating windows, buttons, forms, etc. 
  - Handles user input and displays information to the user. 
**2.Logic Tier (Application Tier):** 
- Manages the application's functionality and business logic. 
- Python code in this tier processes user inputs from the GUI and communicates with the  backend. 
- Ensures the proper flow of information between the presentation and data tiers. 
**3.Data Tier (Back End - MySQL):** 
- Handles data storage and retrieval. 
- Utilizes MySQL to store and manage the application's data. 
- The logic tier communicates with the MySQL database to perform CRUD (Create, Read, Update, Delete) operations. 

**Communication between tiers:** 
- The **presentation tier** interacts with the **logic tier** by triggering events (button clicks, form submissions). 
- The **logic tier** processes these events, performs necessary operations, and communicates with the **data tier** for data storage or retrieval. 
- The **data tier** stores and manages the application's data, responding to requests from the **logic tier**. 

**Benefits of a three-tier architecture:** 
- **Modularity:** Each tier can be developed, maintained, and scaled independently. 
- **Scalability:** It's easier to scale individual components based on demand. 
- **Maintainability:** Changes in one tier have minimal impact on the others. 
## Architecture Diagram

![3-Tier Architecture Diagram](https://i.postimg.cc/jdHxsvh4/3-tier-application-exp8-pdf-Page-2-image-1.png)

## Output Screens
Initially, the screen in MySQL Command Client after creating the database and the table. 

![](https://i.postimg.cc/MpphhY3T/3-tier-application-exp8-pdf-Page-7-image-1.png)

After executing the python file, the GUI Window looks like:

![](https://i.postimg.cc/66Rw0zFx/3-tier-application-exp8-pdf-Page-7-image-2.png)

Now enter the 2 values and click insert.

![](https://i.postimg.cc/52PM0rQL/3-tier-application-exp8-pdf-Page-8-image-1.png)

![](https://i.postimg.cc/5NSJcyxP/3-tier-application-exp8-pdf-Page-8-image-2.png)

After clicking insert, you get:

![](https://i.postimg.cc/nz9xN1z7/3-tier-application-exp8-pdf-Page-8-image-3.png)

Click on OK. 

Then, open MySQL:

![](https://i.postimg.cc/4yCGGh70/3-tier-application-exp8-pdf-Page-8-image-4.png)

When we simply click on delete without entering the values, then we get:

![](https://i.postimg.cc/1XpQ35D3/3-tier-application-exp8-pdf-Page-8-image-5.png)

![](https://i.postimg.cc/MGTqmwJ9/3-tier-application-exp8-pdf-Page-8-image-6.png)


The Alerts are generated when we click on select, insert, delete and update when we do not 
enter the values on the GUI window.

When we want to delete the 2nd row, then click on Delete button:

![](https://i.postimg.cc/YSskXPpM/3-tier-application-exp8-pdf-Page-9-image-1.png)

![](https://i.postimg.cc/wTpzbLdy/3-tier-application-exp8-pdf-Page-9-image-2.png)

Now open MySQL:

View the table

![](https://i.postimg.cc/q7zHCG2Y/3-tier-application-exp8-pdf-Page-9-image-3.png)

Now, enter the values in the GUI Window

![](https://i.postimg.cc/WzcBCLxL/3-tier-application-exp8-pdf-Page-9-image-4.png)

Click on insert

![](https://i.postimg.cc/xCmr6Tx3/3-tier-application-exp8-pdf-Page-10-image-1.png)

Open MySQL, view the table

![](https://i.postimg.cc/KcnSLjgZ/3-tier-application-exp8-pdf-Page-10-image-2.png)

Enter the below values in the GUI Window to update one row in the table

![](https://i.postimg.cc/650kjP0g/3-tier-application-exp8-pdf-Page-10-image-3.png)

Click on Update. 

![](https://i.postimg.cc/vT7Jd2d1/3-tier-application-exp8-pdf-Page-10-image-4.png)

Now, open MySQL Command Line Client.

![](https://i.postimg.cc/28rpxY4n/3-tier-application-exp8-pdf-Page-11-image-1.png)

Open the GUI Window and do as the below:

![](https://i.postimg.cc/g0w102Wb/3-tier-application-exp8-pdf-Page-11-image-2.png)

Click on Select. Then you get the other values automatically in the other text boxes.

![](https://i.postimg.cc/k5kzRPJ6/3-tier-application-exp8-pdf-Page-11-image-3.png)
