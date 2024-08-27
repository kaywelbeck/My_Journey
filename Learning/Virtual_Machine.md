<div style="text-align: center;">
<h1><u>Virtual Machine</u></h1>
</div>

<h4><u>WHAT ARE VIRTUAL MAHCINES?</u></h4>

<h5><span style="color:green;">A Virtual Machine (VM)</span> is a <span style="color:purple;">Software-Based Computer</span></h5>

<div style="display: flex; align-items: flex-start;">
    <img src="https://static.javatpoint.com/cloudpages/images/cloud-hypervisor.png" alt="Cloud Hypervisor" style="width: 400px; height: auto; margin-right: 20px;" />
    <ul>
        <li>A VM runs on a physical computer, which is called a <span style="color:purple;">Host</span></li>
        <li>A software layer, which is called a <span style="color:purple;">Hypervisor,</span> provides access to the resources of the physical computer (CPU, memory, disk, and network) to the VM.</li>
        <li><span style="color:purple;">The VM runs its own operating system (OS)</span> and interacts with the host through the hypervisor.</li>
        <li><span style="color:purple;">Multiple VMs</span> can be provisioned on a single host.</li>
    </ul>
</div>
<span style="color:purple;">Virtualization</span> gives you the ability to create multiple VMs, each with its own OS and applications, on a single physical machine.

A virtual machine (VM) is a computer that is emulated through software. It is virtual because it is not a physical computer. 

---
<h4><u>Benefits of VMs</u></h4>

- <span style="color:green;"> Cost savings –</span> you don’t need to buy a new machine if you want to run a different operating system (OS) on your existing machine. You create a VM with the new OS and run it on your machine with virtualization software.
- <span style="color:green;"> Efficiency –</span> You can run multiple VMs on a single physical computer to handle different types of workloads and increase its utilization. You can use VMs to reduce computing resource waste due to underused servers.
- <span style="color:green;"> Reusability and portability –</span> You can copy aVM image on the same physical host or moveit to a different host to duplicate the VM’s computing environment.

---

<h4><u>VMs in the cloud</u></h4>

<h5><span style="color:green;">VMs are the fundamental unit of computing in the cloud.

- self-service
- scalability
- pay only for what you use
</span></h5>

```mermaid
graph TD
    A[AWS Cloud] --> B[EC2 Instances]
    B --> C[VM1]
    B --> D[VM2]
    A --> E[S3 Storage]



