# DevOps

## What is DevOps?

### Software Developmet Process:

**1) Requirement Gathering and Analysis**

Information will be collected like:
- Product Features
- Users
- Usage
- User Requirement
- Market State

**2) Planning What do we want?**
- COST
- RESOURCES
- RISK

**3) Design Architects**
- Based on detail Requirement System Design Documents are created

**4) Development Developers**
- Software Development Based on inputs of Design Documents

**5) Testing Quality Assurance**
- Identify the defects to ensure the quality product is good

**6) Deployment System Admins**
- Operations works in Deployment of product

**7) Maintenance Changes & Uptime**
- System Health
- Performance Uptime with regular changes

### Softwre Development LifeCycle:

![Screenshot from 2023-10-27 11-35-04](https://github.com/Ankit6989/Devops/assets/114300894/3bc753a9-874b-4f62-932f-49cc3edc0907)

- **Models in SDLC**

In Software Development Life Cycle (SDLC), various models are used to guide the development process. Each model represents a specific approach to how software projects should be planned and executed. Here are some common SDLC models:

1. **Waterfall Model:**
   - The Waterfall model is a linear and sequential approach.
   - It divides the project into distinct phases, such as requirements, design, implementation, testing, deployment, and maintenance.
   - Each phase must be completed before the next one begins.
   - It is suitable for well-defined and stable projects with no or minimal expected changes.

2. **Agile Model:**
   - Agile is an iterative and incremental model that focuses on flexibility and customer collaboration.
   - The project is divided into short development cycles called iterations.
   - Requirements can evolve, and changes can be accommodated at any point in the project.
   - Scrum, Kanban, and Extreme Programming (XP) are some popular Agile methodologies.

3. **Iterative Model:**
   - Similar to Agile, the Iterative model breaks the project into smaller cycles or iterations.
   - Each iteration includes requirements, design, coding, and testing phases.
   - It allows for changes between iterations but provides more structure than Agile.

4. **Spiral Model:**
   - The Spiral model combines iterative and incremental development with elements of the Waterfall model.
   - It focuses on risk assessment and involves multiple cycles, each consisting of four major phases: Planning, Risk Analysis, Engineering, and Evaluation.
   - Well-suited for large and complex projects with high levels of uncertainty and risk.

5. **V-Model (Validation and Verification Model):**
   - The V-Model is an extension of the Waterfall model.
   - Each development phase is associated with a corresponding testing phase.
   - It emphasizes the importance of testing and validation at each step of development.

6. **Big Bang Model:**
   - In the Big Bang model, there is little to no planning, and development begins with little understanding of requirements.
   - It is suitable for small projects or experimental projects where requirements are not well-defined.

7. **Incremental Model:**
   - The Incremental model divides the project into smaller components or modules.
   - Each module is developed and tested independently and then integrated into the main system.
   - This approach allows for partial and early system deliveries.

8. **RAD (Rapid Application Development) Model:**
   - RAD is an adaptive approach that focuses on rapid prototyping and speedy development.
   - It is well-suited for projects with a short timeline and when user feedback is crucial.

9. **DevOps Model:**
   - DevOps, although not a traditional SDLC model, emphasizes the continuous integration and delivery of software.
   - It integrates development (Dev) and operations (Ops) teams to automate and streamline the development, testing, and deployment processes.

It's essential to choose the SDLC model that best suits the specific needs and characteristics of a project. The selection of the model can significantly impact the project's success, so careful consideration is required. Many organizations also customize or combine models to create a tailored SDLC approach.

### DevOps LifeCycle:

![Screenshot from 2023-10-27 11-40-06](https://github.com/Ankit6989/Devops/assets/114300894/80fa8560-617a-4f64-b229-83058e636de2)

## What is Continuous Integration?

- Continuous integration is a software development process where developers integrate the new code they've written more frequently throughout the development cycle, adding it to the code base at least once a day. Automated testing is done against each iteration of the build to identify integration issues earlier, when they are easier to fix , which also helps avoid problems at the final merge for the release. Overall, continuous integration helps streamline the build process, resulting in higher-quality software and more predictable delivery schedules.

**The key goals of continuous integration are:**

- Find and fix bugs earlier in the development process
- Improve software quality through more frequent testing
- Reduce the time it takes to validate and release new software updates

Without continuous integration, developers would have to manually integrate their code changes periodically. This can lead to integration issues, bugs piling up, and slower release cycles.

**With continuous integration, developers benefit from:**

- Faster feedback on code changes through automated testing
- Easier identification and fixing of bugs
- Faster release cycles since integration issues are caught early

**Benefits of continuous integration:**

- Early and improved error detection and metrics that let you address errors early—sometimes within minutes of check-in

- Continuous and demonstrated progress for improved feedback

- Improved team collaboration; everyone on the team can change the code, integrate the system and quickly determine conflicts with other parts of the software

- Improved system integration, which reduces surprises at the end of the software development lifecycle

- Fewer parallel changes for merging and testing

- Reduced number of errors during system testing

- Constantly updated systems to test against

**Continuous integration works by:**

1) Developers committing code changes to a main branch (like main or master) frequently - ideally multiple times a day
2) An automated build is triggered whenever code is committed to the main branch
3) The build compiles the code and runs automated unit and integration tests
4) If the build passes, the code changes are integrated into the main branch
5) If the build fails, developers are notified and they fix the issues before committing again

Tools like Jenkins, Bamboo, GitLab CI, and Azure Pipelines are often used to implement a continuous integration workflow. They integrate with version control systems like Git to trigger automated builds whenever code is committed.

Continuous integration is an essential practice for implementing continuous delivery and DevOps. It helps shorten feedback cycles, improve software quality, and speed up the overall software development process.

![Screenshot from 2023-10-27 12-03-31](https://github.com/Ankit6989/Devops/assets/114300894/f09c1c38-4f0d-498c-a637-05e91bd713fc)
![Screenshot from 2023-10-27 12-05-21](https://github.com/Ankit6989/Devops/assets/114300894/4b2b629c-5e91-41d8-a3e0-4be218b4c010)


## What is Continuous Delivery?

 # What is continuous delivery

Continuous delivery is the practice of automating the process of moving software changes to production. This allows teams to deploy code more frequently, reliably and safely.

The key aspects of continuous delivery are:

- Automating the build, test and deployment pipeline
- Having automated tests to catch errors early 
- Deploying code frequently, even multiple times per day
- Having a production-ready build artifact that has passed all tests
- Deploying to a testing or staging environment first before production
- Having manual approval before deploying to production

The benefits of continuous delivery include:

- Faster time to market for new features
- Higher quality and more stable releases 
- Increased developer productivity 
- Bugs are found and fixed earlier

To implement continuous delivery, teams need:

- Automated build and deployment tools 
- Automated testing (unit tests, integration tests, etc.)
- Infrastucture as code
- Monitoring in place
- Progressive exposure techniques like canary releases and feature flags

Continuous delivery builds on continuous integration by:

- Pushing code changes automatically to a testing environment after tests pass
- Running longer tests like integration, performance and security tests
- Creating multiple testing environments to progressively expose changes

Continuous deployment refers to automatically deploying code changes to production without manual approval. This is a more aggressive form of continuous delivery.

Some tools that can help with continuous delivery are:

- Jenkins
- AWS CodePipeline
- Azure Pipelines
- GitLab CI/CD

In summary, continuous delivery is a DevOps practice that helps teams release software faster and more reliably by automating the process of moving code changes from development to production. It focuses on making every change releasable at any time.

### Continuous integration (CI) vs. continuous delivery (CD) vs. continuous deployment

- Continuous delivery and continuous deployment follow continuous integration in the DevOps cycle. 

- Continuous delivery (CD) picks up where continuous integration ends, automating the delivery of applications to selected infrastructure environments. CD focuses on delivering any validated changes to the code base—updates, bug fixes, even new features—to users as quickly and safely as possible. It ensures the automation of pushing code changes to different environments, such as development, testing and production.

- Continuous Deployment is an extension of Continuous Delivery. In continuous deployment, the code changes to an application are released automatically into the production environment. This automation is driven by a series of predefined tests. Once new updates pass those tests, the system pushes the updates directly to the software's users.

1. **Continuous Delivery (CD):**
   
   - **Definition:** Continuous Delivery is a software development practice where code changes are automatically built, tested, and prepared for release throughout the development cycle. The primary goal of CD is to ensure that the software is always in a deployable state.

   - **Process:** In Continuous Delivery, the software is automatically built and tested at various stages of the development process. If the tests pass, the code is considered ready for deployment but is not immediately deployed to production.

   - **Human Intervention:** CD often includes a manual approval step before the software is deployed to production. This means that human intervention is required to initiate the actual deployment to the production environment.

   - **Benefits:** CD ensures that the software can be reliably and consistently deployed to production at any time. It allows for rigorous testing and quality control before deployment. This practice reduces the risk of deploying faulty code to the production environment.

   - **Use Cases:** Continuous Delivery is commonly used in situations where organizations want to have the flexibility to deploy new features, bug fixes, or updates to production at a pace that suits their business needs.

![image](https://github.com/Ankit6989/Devops/assets/114300894/71dba70b-cb7f-46b1-9878-0155154876b8)


2. **Continuous Deployment (CD):**

   - **Definition:** Continuous Deployment is an extension of Continuous Delivery. In Continuous Deployment, every code change that passes automated tests is automatically deployed to production without manual intervention.

   - **Process:** Unlike Continuous Delivery, where there is typically a manual approval step before production deployment, Continuous Deployment automatically deploys code changes to the production environment as soon as they pass automated tests.

   - **Human Intervention:** Continuous Deployment minimizes human intervention in the deployment process. Once the tests are passed, the deployment happens automatically.

   - **Benefits:** CD is often associated with achieving a high release velocity. It allows organizations to release new features or updates to users rapidly and continuously. This can be a competitive advantage in certain industries.

   - **Use Cases:** Continuous Deployment is common in organizations where rapid and frequent releases are essential, such as web-based services and applications. It is less common in regulated or safety-critical environments where rigorous testing and manual approval are required before deployment.
  
![Screenshot from 2023-10-27 12-21-05](https://github.com/Ankit6989/Devops/assets/114300894/28b2b785-6a04-4c84-8fd3-189c6b34d730)

## VM SetUp:
### Virtualisation:

- Virtualisation is the process of creating a virtual representation of a physical resource, such as a server, storage device, or a network.
- virtualization in a cloud environment offers a lot of benefits to users.

- It enables multiple virtual computers to run on the same physical host computer, each on its own OS and applications.
- It can improve efficiency, scalability, and flexibility of information technology(IT) resources, as well as reduce costs and environmental impact.
- It enables cloud customers to access services over the internet, without having to manage or maintain the underlying physical infrastructure.
- It also enables cloud customers to scale up or down their resources on demand, depending on their needs and requirements.

 ***Cloud Providers Provide 3 types of virtualization***
 - virtual machines
 - virtual storage
 - virtual networks

### Virtual Machines:

The situation changed with development of virtual machines. A virtual machine or VM is a software based emulation of a physical computer that can run different OS and applications.

- Run on a Physical computer and each physical computer can run or host, multiple VMs.
- Have their own virtual hardware, such as CPU, memory, disk, and network devices that are isolated from host system and other VMs.
- Orginally virtual machines were primarily used in business scenarios. But today , the technology is also being regularly used in cloud.

- **Testing and Development**

- **Disaster recovery and backup**

- **Server consolidation**

- **Security and Isolation**

#### How does virtual machine works:

- Virtual machine work with help of virtualization software called a hypervisor.
- The hypervisor manages and allocates the physical resources of the host computer, lke CPU, memory and storage to the virtual machines.

### There are 2 main types of hypervisors:
- **Type 1 Hypervisors(Bare Metal):** Runs directly on the host hardware. They provide the best performance since there are no additional layers between the VM and the hardware.
Eg: Ctrix Hypervisor, Microsoft Hyper-V

- **Type 2 Hypervisors:** Runs with in an OS as an Application. They are easier to install and use but provide slightly worse performance since all VM requests have to go through the host OS first.
Eg: Vm Ware Workstation, Oracle Virtual Box

- The hypervisor abstracts physical hardware and presents virtual hardware to the gurest VMs.
- Thsi allow each VM to run as if it is its own dedicated physical computer.
- The hypervisor schedules and manages the execution of Vms so they can share the host computers resources efficiently.

 #### Main components of VM are:

 - Virtual CPU
 - virtual memory
 - virtual disk
 - virtual network adapter
   
### VM-Manually(LINUX)

1. **Prerequisites for Windows**:
   - Enable virtualization in your computer's BIOS.
   - Ensure that Windows features like Hyper-V, Windows Subsystem for Linux, and Docker Desktop Virtual Machine platform are disabled.

2. **Creating Virtual Machines**:
   - Open Oracle VM VirtualBox from the Start menu.
   - Click on "New" to create a new virtual machine.
   - Give your VM a name, choose the type (Linux), and select the version (e.g., Red Hat 64-bit).
   - Allocate RAM and CPU resources based on your system specifications.
   - Create a virtual hard disk for the VM. You can specify the size (dynamically allocated is recommended).
   - Review the settings and click "Finish" to create the VM.

3. **Downloading Linux ISO**:
   - Download the ISO file for your Linux distribution (e.g., Alma Linux, CentOS, or Ubuntu).

4. **Configuring Virtual Machine Settings**:
   - Attach the downloaded ISO to the virtual optical drive.
   - Set up network settings, especially the bridged adapter, to ensure the VM connects to your router.

5. **Starting the Installation**:
   - Boot the VM, which will automatically boot from the attached ISO.
   - Follow the installation process for the Linux distribution you've chosen. Customize settings as needed, like hostname, password, and software installation options.

6. **Completing the Installation**:
   - After installation, power off the VM.

7. **Testing SSH Access**:
   - Check the IP address of the VM, which is assigned by your router.
   - Open a terminal or command prompt, and use the SSH command to connect to the VM using its IP address and the username and password you specified during the installation.
   - Confirm successful SSH access to the VM.

8. **Shutting Down the VM**:
   - After testing, shut down the VM from within the VM itself or from the Oracle VM VirtualBox interface.

This process allows you to manually set up virtual machines running CentOS and Ubuntu. In subsequent lectures, you'll learn how to automate this process to create and configure VMs more efficiently.

### VM-Automatically(LINUX) Using VAGRANT:

kali Linux does not work














