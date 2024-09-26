<div style="text-align: center;">
    <h1><u>AWS</u></h1>
</div>

<div style="text-align: center;">
    <h2><u>WHAT IS AWS?</u></h2>
</div>

 **AWS** stands for **Amazon Web Services**.
- It's a major player in the tech industry, providing a wide range of cloud computing services.

---

## Key Offerings 💻
- AWS offers **IT infrastructure services** to help businesses scale and grow efficiently.
- Services previously bought as hardware (e.g., network switches, servers) are now available as web resources accessible via the internet.

---

## Benefits of Using AWS 🌟
- **Pay-as-You-Go Model**: Organizations save time, money, and human resources by utilizing AWS.
- **Flexibility, Scalability, and Reliability**: AWS allows for dynamic adjustments to resources, catering to various needs.
- **Focus on Development**: Engineers can concentrate on building products without worrying about underlying infrastructure.

---

## Types of Services Offered ⚙️
As of winter 2020, AWS includes **24 service groups**, each with various services. Here are some examples:
- **Compute**: Elastic Compute Cloud (EC2) for hosting applications.
- **Storage**: Simple Storage Service (S3) for hosting static files.
- **Email**: WorkMail for sending emails.
- **Virtual Desktops**: WorkSpaces for streaming desktop environments.
- **Game Development**: GameLift for creating and hosting games.

---

## Conclusion
AWS empowers organizations with the ability to architect a wide array of solutions, limited only by imagination. Its affordability and robust resources make it a compelling choice for cloud computing.

git ---

# ☁️ AWS Cloud Adoption Framework (AWSCAF)

---

## Overview
- **IT Infrastructure Migration**: Organizations can build directly in AWS or migrate existing infrastructures to the AWS cloud, known as cloud adoption.
- **AWSCAF Purpose**: Identifies best practices for successfully migrating IT infrastructure to the cloud.

---

## Key Concepts of AWSCAF

### Transformation Domains 🔄
AWSCAF outlines a value chain where transformations in one domain enable transformations in the next:

1. **Technological Transformation**: 
   - Migrate and modernize legacy infrastructure, applications, and data analytics platforms.
   
2. **Process Transformation**: 
   - Digitize, automate, and optimize business operations.

3. **Organizational Transformation**: 
   - Reimagine how business and technology teams collaborate to create customer value.

4. **Product Transformation**: 
   - Innovate business models to create new value propositions and revenue streams.

### Desired Business Outcomes 🎯
- **Reduced Business Risk**
- **Improved Environmental, Social, and Governance Performance**
- **Revenue Growth**
- **Increased Operational Efficiency**

---

## Foundational Capabilities 🏗️
AWSCAF organizes capabilities into six perspectives that help organizations deploy resources effectively:

1. **Business Perspective**:
   - Focus: Accelerate digital transformation and outcomes.
   - Stakeholders: CEO, CFO, COO, CIO, CTO.
   - Capabilities: Strategy management, product management.

2. **People Perspective**:
   - Focus: Foster a culture of continuous growth and learning.
   - Stakeholders: CIO, COO, CTO, Cloud Director.
   - Capabilities: Cloud fluency, organization design.

3. **Governance Perspective**:
   - Focus: Maximize benefits while minimizing risks.
   - Stakeholders: Chief Transformation Officer, CIO, CTO, CFO.
   - Capabilities: Risk management, data governance.

4. **Platform Perspective**:
   - Focus: Build scalable hybrid cloud platforms and modernize infrastructure.
   - Stakeholders: CTO, Technology Leaders, Architects.
   - Capabilities: Platform engineering, modern application development.

5. **Security Perspective**:
   - Focus: Ensure data confidentiality, integrity, and availability.
   - Stakeholders: CISO, Chief Compliance Officer, Security Architects.
   - Capabilities: Security governance, threat detection.

6. **Operations Perspective**:
   - Focus: Ensure cloud services meet business needs.
   - Stakeholders: Infrastructure Leaders, Site Reliability Engineers.
   - Capabilities: Observability management, incident management.

---

## Cloud Transformation Journey 🚀
To ensure effective cloud adoption, organizations should:

1. **Envision**: Demonstrate how cloud adoption accelerates outcomes.
2. **Align**: Identify capability gaps and stakeholder concerns across AWSCAF perspectives.
3. **Launch**: Deliver pilot initiatives to demonstrate incremental business value.
4. **Scale**: Expand pilots to meet business needs while sustaining benefits.

---

## Additional Resources
For more detailed information on AWSCAF, visit: [AWS Cloud Adoption Framework](https://aws.amazon.com/cloud-adoption-framework) for eBooks, infographics, and more.

---

## Summary
The AWS Cloud Adoption Framework provides a structured approach to cloud migration, focusing on best practices across transformation domains and foundational capabilities to achieve optimal business outcomes.

---

<div style="text-align: center;">
    <h2><u>AWS PRICING</u></h2>
</div>

<ul>
    <li>COMPUTE - calculated either by hour or by second</li>
</ul>

---

<div style="text-align: center;">
    <h2><u>AWS Infrastructure</u></h2>
</div>

<img src="https://d2908q01vomqb2.cloudfront.net/da4b9237bacccdf19c0760cab7aec4a8359010b0/2020/03/17/aws_regions-1.png" alt="AWS Global Infrastructure" style="border: 2px solid black;" height="350"/>

<p>The AWS Global Infrastructure is designed and built to deliver:</p>
<ul>
    <li><span style="color: green;">A flexible</span></li>
    <li><span style="color: green;">Reliable</span></li>
    <li><span style="color: green;">Secure cloud computing environment with high-quality global network performance.</span></li>
</ul>

<h4><u>AWS Availability</u></h4>

<img src="Screenshot 2024-08-23 110025.png" alt="AWS Availability" style="border: 2px solid black;" />

<h5>The AWS Global Infrastructure consists of three elements:</h5>
<ul>
    <li><span style="color: green;">Regions</span></li>
    <li><span style="color: green;">Availability Zones</span></li>
    <li><span style="color: green;">Points of presence (PoPs)</span></li>
</ul>

<h4><u><span style="color: green;">The foundation for the AWS infrastructure is the data centers</span></u></h4>
<p>Data centers usually have specific characteristics:</p>
<ul>
    <li>They are a location where the actual physical data resides and data processing occurs.</li>
    <li>They house physical servers (typically 50,000 to 80,000 servers).</li>
    <li>They are online. They are never cold (not in use).</li>
</ul>

---

<div style="text-align: center;">
    <h2><u>AWS Shared Responsibility Model</u></h2>
</div>

<img src="https://d1.awsstatic.com/security-center/Shared_Responsibility_Model_V2.59d1eccec334b366627e9295b304202faf7b899b.jpg" alt="AWS Shared Responsibility Model" height="350" width="1000"/>

<h5><span style="color: green;">AWS</span> is responsible for <span style="color: green;">SECURITY OF THE CLOUD</span></h5>

<h5><span style="color: green;">CUSTOMERS (YOU)</span> are responsible for <span style="color: green;">SECURITY IN THE CLOUD</span></h5>

<h4><u><span style="color: green;">SECURITY OF THE CLOUD</span></u></h4>

<table>
    <thead>
        <tr>
            <th>IaaS</th>
            <th>PaaS</th>
            <th>SaaS</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Col 1</td>
            <td>Row 1, Col 2</td>
            <td>Row 1, Col 3</td>
        </tr>
        <tr>
            <td>Row 2, Col 1</td>
            <td>Row 2, Col 2</td>
            <td>Row 2, Col 3</td>
        </tr>
        <tr>
            <td>Row 3, Col 1</td>
            <td>Row 3, Col 2</td>
            <td>Row 3, Col 3</td>
        </tr>
    </tbody>
</table>

---

<div style="text-align: center;">
    <h2><u>S3 Bucket</u></h2>
</div>

<ul>
    <li>Data is stored as <span style="color: green;">Objects</span> in <span style="color: green;">Buckets</span>.</li>
    <li>Storage is virtually unlimited.</li>
    <li>A single object can be up to 5 TB.</li>
    <li>Amazon S3 is designed for 11 9s (99.999999999 percent) of durability.</li>
    <li>Customers have granular access to buckets and objects.</li>
</ul>


 ---

 <div style="text-align: center;">
    <h2><u>EC2Amazon Elastic Compute Cloud (Amazon EC2)</u></h2>
</div>

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

Amazon EC2's simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon's proven computing environment. Amazon EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.

Amazon EC2 changes the economics of computing by allowing you to pay only for capacity that you actually use. Amazon EC2 provides developers the tools to build failure resilient applications and isolate themselves from common failure scenarios.

steps:
- Step 1: Naming your EC2 instance
- step 2: Choosing an Amazon Machine Image (AMI)
- Step 3: Choosing an instance type
- Step 4: Configuring a key pair
- Step 5: Configuring the network settings 
- Step 6: Adding storage