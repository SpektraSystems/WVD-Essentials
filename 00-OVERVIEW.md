# **Overview** 
   
Windows Virtual Desktop is a desktop and app virtualization service that runs on the cloud.

Here's what you can do when you run Windows Virtual Desktop on Azure:

   - Set up a multi-session Windows 10 deployment that delivers a full Windows 10 with scalability.
   - Virtualize Microsoft 365 Apps for enterprise and optimize it to run in multi-user virtual scenarios.
   - Provide Windows 7 virtual desktops with free Extended Security Updates.
   - Bring your existing Remote Desktop Services (RDS) and Windows Server desktops and apps to any computer.
   - Virtualize both desktops and apps.
   - Manage Windows 10, Windows Server, and Windows 7 desktops and apps with a unified management experience.

## **General Hierarchy**

### **Host Pools**

Host pools are a collection of one or more identical virtual machines within Windows Virtual Desktop tenant environments. Each host pool can be associated with multiple RemoteApp groups, one desktop app group, and multiple session hosts. Host Pools can be one of two types: 

   - **Personal**, where each session host is assigned to individual users. 
   - **Pooled**, where session hosts can accept connections from any user authorized to an application group within the host pool. You can set additional properties on the host pool to change its load-balancing behavior, how many sessions each session host can take, and what the user can do to session hosts in the host pool while signed in to their Windows Virtual Desktop sessions. You control the resources published to users through application groups. 


### **Application Groups**

An Application group is a logical grouping of applications installed on session hosts in the host pool. An application group can be one of two types: 

   - **RemoteApp**, where users access the RemoteApps you individually select and publish to the application group. 
   - **Desktop**, where users access the full desktop By default, a desktop application group (named “Desktop Application Group”) is automatically created whenever you create a host pool. You can remove this application group at any time. However, you can’t create another desktop application group in the host pool while a desktop application group already exists. To publish RemoteApps, you must create a RemoteApp application group. You can create multiple RemoteApp application groups to accommodate different worker scenarios. Different RemoteApp application groups can also contain overlapping RemoteApps. 


### **Workspaces** 

A workspace is a logical grouping of application groups in Windows Virtual Desktop. Each Windows Virtual Desktop application group must be associated with a workspace for users to see the remote apps and desktops published to them. 

### **End users**

After you’ve assigned users to their application groups, they can connect to a Windows Virtual Desktop deployment with any of the Windows Virtual Desktop clients. 

________________________________________________





# Lab Outline

**Overview**

**Pre-requisites to deploy Windows Virtual Desktop**

**Exercise 1: Create Host Pool from Azure Portal**

- Task 1: Log in to Azure Portal
- Task 2: Create Host Pool
    
**Exercise 2: Create Application Groups and assign to users**
    
- Task 1: Create Application Group
    
**Exercise 3: Access the Published Applications and Desktop using Browser**

- Task 1: Access the Published Application
- Task 2: Access the published Desktop
    
**Exercise 4: Access the Published Applications and Desktop using WVD Desktop Client**
    
- Task 1: Access the Published Applications
- Task 2: Access the Virtual Desktop
    
**Summary**


Click on the **Next** button present in the bottom-right corner of this lab guide.  
