# AWS Beginner Guide to Configuration and DevOps Concepts

---
<img src="https://docs.aws.amazon.com/images/whitepapers/latest/best-practices-building-data-lake-for-games/images/mwaa.jpg">

### 1. What is Configuration Orchestration?
Configuration orchestration is about organizing and managing the setup of all parts of a computing environment automatically. Imagine you're setting up a computer game; instead of adding every setting manually, configuration orchestration is like using a tool that sets up everything for you so it all works smoothly. In AWS, this means using tools to manage lots of resources so they interact well together, without needing to manually configure each part.
---
<img src="https://maturitymodel.security.aws.dev/en/Config1.png">

### 2. What is Configuration Management?
Configuration management is the process of keeping track of and managing the setup (or “configuration”) of your systems over time. AWS provides tools to help manage settings on things like servers and networks to ensure they work reliably and stay consistent. process of ensuring that the configurations of a system’s servers, applications, and other environments remain known, consistent, and trusted over time. Any IT system has certain configurations related to software versions, security, networking, and other settings that are essential for optimal functioning. Configuration management tracks, updates, and maintains these configurations so that the system performs at a predetermined baseline and remains secure despite any changes.

### benifts

#### Improve system recoverability
-  With configuration management, you can prevent service disruption by recovering and reverting to previously working configuration values. 

#### Reduces system disruption
- Misconfigured software results in service breakdown. A configuration management system documents and stores all configuration changes in a centralized platform. You can recreate the environment where failure was detected for further analysis. This facilitates remediation efforts and reduces costly system breakdowns.

#### Accelerate software development
- With configuration management tools, you can automate, observe, and analyze configuration settings in test and production environments. You can simulate production environments easily by adding parameter changes without overwriting baseline values.

---

<img src="https://digitalcloud.training/wp-content/uploads/2022/01/AWS-Systems-Manager-400x200.jpg">

### 3. List Some Commonly Used Tools for Configuration Management
Here are some popular tools:
- **AWS Systems Manager**: A tool for organizing and managing AWS setups.
- **Puppet** and **Chef**: These automate the setup and management of large-scale infrastructure, like setting up software and servers.
- **Ansible**: Known for being easy to use, Ansible can automate the setup of systems in both cloud and on-premises environments.

---

### 4. What is Continuous Integration (CI)?
Continuous Integration, or CI, is a practice where developers constantly upload their code changes to a shared place where it gets automatically tested. Think of it like uploading an assignment to a shared folder where it’s immediately checked for errors. This way, everyone on the team can catch mistakes early and make sure new features are working well with the old ones. In AWS, CodeBuild and CodePipeline are tools that help make this happen.

<img src="https://civo-com-assets.ams3.digitaloceanspaces.com/content_images/2585.blog.png?1704705311">

### 5. What is Continuous Delivery (CD)?
Continuous Delivery, or CD, is a way to ensure that code is always ready to go live as soon as it passes tests. It’s like making sure your game character is ready for battle at any moment by automatically preparing them with the latest armor and skills! AWS tools like CodePipeline and CodeDeploy help automate this process so you can quickly release code updates to users.

---
<img src="https://digitalcloud.training/wp-content/uploads/2022/01/AWS-CloudFormation-600x300.jpg">

### 6. What is AWS CloudFormation?
AWS CloudFormation is like a blueprint or template that tells AWS exactly what resources to create and how to connect them. Instead of manually setting up each part (like storage, servers, and databases), you write down instructions in a template (file) and CloudFormation creates everything for you based on those instructions. It saves a lot of time and helps prevent mistakes.

### 7. List 3 Advantages of CloudFormation
1. **Automation**: CloudFormation automatically sets up, updates, and deletes resources, which saves time and reduces errors.
2. **Consistency**: Using templates ensures that the setup is always done in the same way, no matter how many times you deploy it.
3. **Less Work**: CloudFormation takes care of connecting different resources and managing changes, so you can focus on the bigger picture instead of individual details.

---
<img src="https://media.licdn.com/dms/image/v2/D5612AQHg0innTm-Uhw/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1708953765680?e=2147483647&v=beta&t=DOrYrI__9tno3LLJlTgWrLl-k8yB_OpJqnmMipr7Ldk">

### 8. What are JSON and YAML?
JSON and YAML are two types of file formats used to organize data. Both can be used to write instructions for CloudFormation templates. You can think of them as different languages for giving AWS instructions on what to create and manage:
- **JSON** (JavaScript Object Notation) uses curly braces `{}` and is often a little more technical.
- **YAML** (YAML Ain't Markup Language) is simpler and often easier to read because it uses indentations instead of braces.

### 9. List 3 Differences between JSON and YAML
1. **Appearance**: JSON uses `{}` and `[]` symbols, while YAML just uses indentation and `-` for lists, making it look cleaner.
2. **Length**: YAML files are shorter because they don’t need as many symbols or quotes as JSON.
3. **Readability**: YAML is often easier to read and understand at a glance, especially for beginners, whereas JSON is a little more complex but has strong support across programming languages.
---
<img src="https://docs.aws.amazon.com/images/AWSCloudFormation/latest/UserGuide/images/stack_set_conceptual_sv.png">

### 10. What is a Stack in AWS CloudFormation?
A stack in AWS CloudFormation is a group of AWS resources (like databases, servers, and networks) that are created and managed together. Think of it as a box of building blocks that you can set up all at once based on instructions you provide in a template. This makes it easy to create, update, or delete multiple resources at the same time.
