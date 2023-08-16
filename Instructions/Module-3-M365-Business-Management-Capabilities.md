# Module 3: M365 Business Management Capabilities 

 In this module, you will learn to work with M365 groups, Microsoft Planner, Forms, Power BI. You will also explore through Microsoft Endpoint Manager.

#  Types of Groups in M365 

1. In the Groups section of the Microsoft 365 admin center, you can create and manage different types of groups:

   - **Microsoft 365 group**:  Microsoft 365 groups are used for collaboration between users, both inside and outside your company. With each Microsoft 365 group, members get a group email and shared workspace for conversations, files, and calendar events, and a Planner.
   
   - **Distribution**: Distribution groups are used for sending notifications to a group of people. They can receive an external email if enabled by the administrator.
   Distribution groups are best for situations where you need to broadcast information to a set group of people.
   
   - **mail-enabled security**: These groups are used for granting access to resources such as SharePoint, and emailing notifications to those users.
   
   - **Security groups**: They can be used for granting access to resources such as SharePoint sites. They can make administration easier because you need to only administer the group rather than adding users to each resource individually.
   
# Exercise 1: Create M365 Groups

  In this exercise, you will learn how to create groups and add members to it from the admin center.

### Task 1: Create Office 365 Users [Read-Only]

1. Open a new browser window and log in to the admin center at https://admin.microsoft.com.

3. From the navigation menu, click on the **Users (1)** icon and click on **Active users (2)**. This will display the list of active users.

    ![](Images/ms900-lab1-3-img1.png)

4. Now to create a new user, from the navigation menu click on **Users icon (1)** and click on **Active users (2)**, and then select **Add a user (3)** icon.

    ![](Images/ms900-lab1-3-img3.png)

5. In the **Set up the basics pane**, fill the following details, and then select **Next**.

   - **First name:** Odl

   - **Display Name:** Odl_User-<inject key="DeploymentID" enableCopy="false" />

    - **Username:** Odl

    ![](Images/ms-900-lab1-img2.png)
     
   - **Automatically create a password**: unselected

   - **Password**: Enter a strong password
   
6. In the  **Assign product licenses**  pane, choose your location from the **select location** dropdown. In the licenses section, choose **Assign user a product license** and select **office 365 E5** license. Click **Next**.

     ![](Images/img6.png ) 

7. In the **Optional settings**  pane, leave everything as default and click on **Next**.

    ![](Images/ms900-lab1-img6.png)

8. In the **Review and Finish** pane, review the new user&#39;s settings and click on **Finish adding**, then **Close**.

    ![](Images/ms900-lab1-img7.png)
   
9. Verify that the user has been created successfully. In the Microsoft 365 admin center, in the left navigation pane, select **Users** and select **Active users**. The new user should be listed, along with their assigned license.


### Task 2: Create Office 365 Groups

1. Open a new browser window and log in to the admin center at https://admin.microsoft.com.

1. From the navigation menu click on the **Teams & Groups (1)** icon and click on **Active teams & groups (2)**. Under **Teams & Microsoft 365 groups**, select **+ Add a Microsoft 365 group**.

    ![](Images/MS-900-Mod-3-teams&groups.png)

    ![](Images/MS-900-Mod-3-(m365).png)

12. On the Basics page, type a name for the group as **Sales-demo** and a description(optional). Click **Next**.

    ![](Images/MS-900-Mod-3-basics.png)   

13. On the **Owners** page, choose the name of ODL user who will be designated to manage the group, then select **Add**. Anyone who is a group owner can add or remove members and have unique permissions like the ability to delete conversations from the shared inbox or change different settings about the group. Click **Next**.
 
    ![](Images/M3E2T1Step601.png) 
  
    ![](Images/MS-900-Mod-3-users.png)  
   
14. Now in the **Members** page, select **Add members**, select ODL user, click on **Add**, and then click **Next**. (**Note:** you can join 20 member including owner) 
   
    ![](Images/MS-900-Mod-3-users.png)

15. Now in the **Settings** page, type a unique email address for the group, choose a privacy option based on your requirement, and whether you want to add Microsoft Teams for the group, and then click **Next**.

16. Review your settings and make any changes if needed, select **Create group**, and then **close**.

    ![](Images/MS-900-Mod-3-finish.png)

17. In the admin center, select the name of the group that you want to add members to. Refresh the page if you are not able to see the newly created group.

18. To add members to the group, navigate to the **Membership tab (1)** and select **Members (2)**.

    ![](Images/MS-900-Mod-3-salesdemo.png)
   
19. Click on **+ Add members**, select the users you want to add, and then click on **Save**.
   
20. To learn more about groups refer to https://docs.microsoft.com/en-us/microsoft-365/admin/create-groups.

# Exercise 2: Explore Microsoft Planner 

Microsoft Planner provides a hub for team members to create plans, organize, and assign tasks to different users, and to check updates on progress through dashboards. It also provides a centralized place where files can be shared and give visibility to the whole team.

In this exercise, you will learn how to create a new plan in Microsoft Planner and add members to it, create buckets, add tasks to the bucket and assign the tasks to the user.

1. In the Office365 portal click on the **App launcher** at the top left corner.
 
1. click on **Explore all your apps** and in the search bar search for **Planner**, this will redirect you to the **Planner** web page.
    
1. On **Welcome to Planner** window, Click **>**.
 
    ![](Images/planner1.png)

1. Again on **Plan together** window, Click **>**.
  
    ![](Images/planner2.png)

1. On **Put it on the board** window, click on **Create a plan!** to create your new plan. 

    ![](Images/planner3.png)

1. On the **New plan** window, select **New blank plan** option.

    ![](Images/blank.png)

1. In the **New blank plan** window: 
    
    - Enter a name for the plan as **Demo-plan**.
    
    - Make the plan public if you want it to be visible to the rest of your organization and in search results or make it private if you want only plan members to see it.
    
    - Click on **Add to an existing Microsoft 365 Group** to create your plan in an existing group ( i.e. **Sales-demo**) or if needed you can create a new group.
    
    - Select **Create**.
    
    ![](Images/MS-900-Mod-3-planner.png)

1. Now to add members to the plan, from the upper-right corner of the Planner window click on **Members**. 

    >**Note**: Perform this step only if members are not added to the plan.

1. Search with the ODL email address and select the person's card when it appears.

1. Now to create a bucket click on **Add new bucket**. Buckets helps to organize tasks into things like workstreams, project phases, or topics. 

1. Type a name for the bucket, and then press Enter.

1. Select **Add task** below the heading of the bucket to which you want to add a task.
    
    - Provide a task name
    
    - Set a due date for the task
    
    - Click on **Assign** and choose a plan member from the list. Type a ODL email address in the search box to add. click on Add task 
    
    ![](Images/MS-900-Mod-3-task.png)
 
1. Click on the task to open the task window. 
 
1. Select **Start anytime** below Start date, and then select the start date you want. Select **Due anytime** below Due date, and then select the due date you want.
 
    ![](Images/MS-900-Mod-3-(startdate).png)
     
1. In the task window select **Priority**  from here you can set the priority of the task.
 
1. Select **Add attachment**. Select **From computer** to attach a locally stored file, select **Link** to include a link, or select **SharePoint** to attach a file from a SharePoint site.

    ![](Images/image10.png)

1. Navigate to and select the file you want to attach or enter any link information and click on **Add**.

1. You can also add comments in **Comment** section. When done click on the dismiss button in the upper-right corner of the task window to save and close the task.

1. Now select **Charts**. The charts show how your plan is progressing, with details about what’s done, in progress, not started, and late.

    ![](Images/img237.png)

1. To learn more about planner refer to https://support.microsoft.com/en-us/planner.

# Exercise 3 : Setup Microsoft Forms 

This exercise explains how to create and work with Microsoft Forms.
 
### Task 1 : Creating a new Form

With Microsoft Forms, you can create surveys, quizzes, and polls, and easily see results as they come in.

In this task, you will learn how to create a Form using Microsoft Forms.

1. Open a browser where admin center page is opened.

1. In the office365 portal from the **App launcher** click on **Explore all your apps** and in the search bar search for **Forms**, this will redirect you to the **Forms** web page.

1. Select **+ New Form** to begin creating your form.

    ![](Images/form.png)

1. Enter a name **Demo** for your form, you can also enter a description if needed.

1. Click **+ Add New** to add a new question to the form. 

    ![](Images/MS-900-Mod-3-demo.png)

1. Choose from Choice, Text, Rating, or Date questions. You can also click More question types Drop down list for more question types in Microsoft Forms to select Ranking, Likert, File upload, or Net Promoter Score® questions. 

    ![](Images/img67.png)

1. For now select **Choice**. Enter the text you want to display for the question and each of the choices. Click **+ Add Option** to add more choices than the default two choices.

1. Click **+ Add New** to add more questions to your form. Now select **Text**.

1. For text questions, select the **Long Answer** option if you want a larger text box displayed on the form.

1. Text questions also allow you to set restrictions when you need to have numbers as the answer. For this click on **More options** button, and then select **Restrictions**.
    
    ![](Images/img68.png)
   
    ![](Images/img69.png)
  
1. Now from the drop-down select **Between** and enter the number. You can choose to restrict the numbers by selecting from the various options such as Greater than, Less than, Between, and many others.
   
    ![](Images/img70.png)

1. Click Preview at the top of the design window to see how your form will look on a computer. Now to test your form, enter answers for the questions in preview mode and then click on **Submit**.

1. Now click on **Back** and select the **Responses tab**. From here you can see summary information data about your form, such as the number of responses and the average time it took for respondents to complete your form.

    ![](Images/MS-900-Mod-3-responses.png)

### Task 2 : Change a form Style and Sharing forms

In this task, you will learn how to customize the theme of your newly created form and the means to share it.

1. Click on the **Style** at the top right of the design window and pick the color or background you want.

    ![](Images/MS-900-Mod-1-styles.png)

1. If you prefer to customize the style, within the style page scroll down and select **+ Customize theme** button. From here you can either upload an image by clicking on **Upload image** icon or customize the color of your choice by clicking on **Customize color** button.

    ![](Images/img75.png)

1. From the top navigation menu click on **Collect Responses**. From here based on your requirement you can either use a link, QR code, Embed, or Email option to share your form.
   
1. To know more about forms refer to https://support.microsoft.com/en-us/forms.

# Exercise 4 : Setup Basic PowerBI Report from a sample Excel 

In this exercise, you will learn how to create a Power BI report from sample data and visualize it.

### Task 1: Import data to PowerBI

In this task, you will import sample financial data to PowerBI. 

1. Open a browser where admin center page is opened.

1. In office365 portal from the **App launcher** click on **Explore all your apps** and in the search bar search for **Power BI**, this will redirect you to the **Power BI** web page.

1. Download sample data from https://docs.microsoft.com/en-us/power-bi/create-reports/sample-financial-download

     ![](Images/MS-900-Mod-1-directly.png)
   
1. In Power BI, from the left navigation menu select **My workspace**.

    ![](Images/MS-900-11.png)
  
1. Click on **Upload**, and from the drop-down select **Browse**.
 
    ![](Images/MS-900-12.png)
    
1. Browse to where you saved the Financial Sample data file, and click on **Open**.


### Task 2 : Visualize data

In this task, you will visualize the data which you had imported in the previous task by using various visualization options available in PowerBI.

1. Go to setting in power Bi, click on Admin Portal, further search for map and enable the **Use Azure Maps visual** Apply.

    ![](Images/MS-900-13.1.png)
    
1. Similarly, enable the **Map and Filled map visuals** and Apply.
    
    ![](Images/MS-900-14.png)
    
1. Go to My workspace and Click on **New (1)** from the drop-down Select **Dataset (2)**.
    
    ![](Images/dateset.png)
    
1. On **Add date to start building a report** window, Select **Excel**.

    ![](Images/excel.png)
   
1. On **Select a file** window, Click on **Browse this device**.

    ![](Images/browsfile.png)
    
1. Select previously downloaded **Financial Sample** excel.

   ![](Images/selectexcel.png)
            
1. Go to My workspace and click on **Financial Sample** dataset. From the dropdown of **+Create a report (1)**, click on **Start from scratch (2)**.

    ![](Images/fromscrach.png)

1. The report opens in the Editing view and displays the blank report canvas. On the right are the **Visualizations**, **Filters**, and **Data** panes.

    ![](Images/FVD.png)

1. Now let us create visualizations (1) by selecting **Clustered column chart (2)**. Let's say your manager wants to see profit over time. To do this, From Data (3) pane, select **Date (4)**. Power BI updates the column chart to show profit by date, in the Dataf pane select **Profit (5)**. Power BI displays a column chart with one column.

    ![](Images/graph.png)
  
1. We can also create a map visualization. In this, we will check which countries are the most profitable.

1. Select a blank area on your report canvas and click on **Maps (2)** under visualization (1) pane. From the **Data (3)** pane, select **Country (4)**, and **Profit (5)** field. Power BI creates a map visual with bubbles representing the relative profit of each location.

    ![](Images/map.png)

1. In this way you can explore through other visualization options.

1. To save your report from the top navigation menu, select **File (1)** and click on **Save (2)**, provide a name for your report, and select **Save**.

    ![](Images/save.png)

1. To learn more about **Power BI** refer to https://docs.microsoft.com/en-us/power-bi/fundamentals/power-bi-overview.

# Exercise 5 : Explore Microsoft EndPoint Manager 

Microsoft Endpoint Manager helps deliver the modern workplace and modern management to keep your data secure, in the cloud and on-premises. Endpoint Manager includes the services and tools you use to manage and monitor mobile devices, desktop computers, virtual machines, embedded devices, and servers. Endpoint Manager combines services like Microsoft Intune, Configuration Manager, Desktop Analytics, co-management, and Windows Autopilot.

In this exercise, you will explore various available options in Microsoft EndPoint Manager.

Before we explore the Microsoft EndPoint Manager, we need to activate the **Enterprise Mobility + Security e5** license in order to view the **Endpoint Manager**.

1. Open a browser where admin center is opened.

1. From the navigation menu , select **Billing**, and select **Licenses**.

    ![](Images/MS-900-Mod-3-billing.png)

1. Select the **Enterprise Mobility + Security E5** license, select **+ Assign licenses**, search and select the ODL user, and click on **Assign**.

1. Switch back to **Admin Center** portal. Refresh your browser window. Select **Show all** Now from the navigation menu scroll down to Admin centers, and select **Endpoint Manager**. This will redirect you to the Endpoint Manager admin center.

    ![](Images/img196.png)

1. From the navigation pane, select **Dashboard** to display overall details about the devices and client apps in your Intune tenant.

    ![](Images/img197.png)

1. Microsoft Intune is a cloud-based service that focuses on mobile device management (MDM) and mobile application management (MAM). Intune is part of Microsoft's Enterprise Mobility + Security (EMS) suite.

1. From the navigation pane, select **Devices**  to display details about the enrolled devices in your Intune tenant.

1. The Devices, **Overview** pane has several tabs that allow you to view a summary of the following statuses and alerts:

      -  **Enrollment status** - Review details about Intune enrolled devices by platform and enrollment failures.
      
      -  **Enrollment alerts** - Find more details about unassigned devices by platform.

      -  **Compliance status** - Review compliance status based on device, policy, setting, threats, and protection. Additionally, this pane provides a list of devices without a compliance policy.

      - **Configuration status** - Review configuration status of device profiles, as well as profile deployment.
      
      - **Software update status** - See a visual of the deployment status for all devices and all users.
      
      ![](Images/img198.png)

1. From the Devices **Overview** pane, select **Compliance policies**  to display details about compliance policies for devices managed by Intune. Compliance requirements are essentially rules, such as requiring a device PIN or requiring device encryption. Device compliance policies define the rules and settings that a device must follow to be considered compliant.

    ![](Images/img200.png)

1. From the Devices Overview pane, select **Conditional Access**, and select **+ Create New Policy** to see all the options available. Now select **X** to exit out of **New -Conditional Access policy** pop up.

   Conditional Access refers to ways you can control the devices and apps that are allowed to connect to your email and company resources.

    ![](Images/ca.png)

1. From the navigation pane, select Devices and select **Configuration profiles** to display details about device profiles in Intune(**Reference**). 

    ![](Images/img201.png)

1. From here you can configure device restriction settings like Allow or block the device camera, control access to Google Play, app stores, viewing documents, and gaming, and much more.

1. In the  **Devices** page select **All devices** to display details about your Intune tenant's enrolled devices. This list of devices show key details about compliance, OS version, and last check-in date. 

    ![](Images/img202.png)
  
    >**Note:** You will not see any devices present in your lab environment. 

1. From the navigation pane select **Apps**. On the apps page select **All apps** this displays a list of apps that have been added to Intune. You can add a variety of different app types based on the platform to Intune. Once an app has been added, you can assign it to groups of users.

    ![](Images/img203.png)

    >**Note:** You will not see any apps present in your lab environment. 

1. From the navigation pane, select **Users** to display details about the users that you have included in Intune.
    
    >**Note:** You will have different list of users in your environment.

1. From the navigation pane, select **Groups** to display details about the Azure Active Directory (Azure AD) groups included in Intune. As an Intune admin, you use groups to manage devices and users.

    >**Note:** You will have different list of groups in your environment.
     
1. To learn more about Endpoint Manager refer to https://docs.microsoft.com/en-us/mem/intune/fundamentals.

## Conclusion

With the help of this module, you learned how to create M365 groups, forms, plans and assign tasks using Planner, also visualized sample data using Power BI and explored through EndPoint Manager
