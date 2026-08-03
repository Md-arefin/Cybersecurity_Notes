# Virtualization

<b>Learning Objectives</b>:

- Understand why managing applications on individual physical servers is inefficient.

- Learn how virtualization addresses hardware utilization and scalability challenges.

- Understand the components of a lab machine.

- Learn how containers have further optimized hardware utilization for applications.


Before the concept of virtualization, the rule of thumb in IT was:
“One server = one application.”

###  <b>Hypervisor</b>

A virtualization layer, called a <b>hypervisor</b>, was introduced to act as a referee between lab machines and allow each virtual computer to behave independently, like a physical computer.

A hypervisor is the core technology behind virtualization. It's the software that creates and manages lab machines.

It is a special piece of software that:

- Divides a physical computer into multiple virtual ones.

- Gives each lab machine its own share of CPU, memory, and storage.

- Keeps everything isolated and safe.

- Manages the lifecycle of lab machines (start, stop, pause, clone, delete).


Hypervisors have two main types of implementation, each of which is used for specific scenarios, from home labs to large data centers:

- <b>Type 1</b> hypervisors run directly on the physical hardware, making them fast, efficient, and ideal for servers and professional environments.

- <b>Type 2</b> hypervisors run within an existing operating system, making them easier to install and ideal for learning, testing, or small setups.

Room Quiz:
1. What is the name of the software that manages the resources for each lab machine?

   = <b>Hypervisor</b>

2. What does virtualization enable multiple applications to share?

    = <b>Physical server</b>

### Lab Machines
A Lab Machine (VM) is a virtual computer created by the hypervisor.
Even though it’s virtual, it behaves as a real machine:

- It has its own virtual CPU, RAM, storage, and network.
- It can run any operating system (Windows, Linux, etc.).
- It’s completely isolated from other VMs. This means that if one VM breaks, the others continue to work.

### Containers 

A container is a lightweight, isolated environment that runs a single application and all the necessary components to support it. Instead of bringing a whole separate operating system, a container borrows the core of the existing system by running on the kernel, which is the part of an operating system that communicates with the hardware and manages resources such as memory and running programs.

Because containers share this kernel, they start quickly and use fewer resources than full lab machines, but it also means they must match the host system’s type. For example, you can’t run a Windows container on a Linux machine.

Containers behave like small, self-contained spaces because:
- They package the application and its dependencies (libraries, tools, versions).
- They share the host’s operating system, so they start almost instantly.
- They remain isolated from each other, so a misbehaving container doesn’t affect the others.
- They can run consistently on any machine, making them perfect for development, testing, and scalable deployments.

The easiest way to deploy containers in a VM is using Docker.

Docker is an open-source software platform that simplifies the process of building, deploying, and running applications using containerization.

Room's Quiz:
1. Suppose a company wants to host multiple small applications in the same lab machine. What should they use?

    = Containers


### Key Terminology

Let's quickly review some concepts we learned in this room:

- Virtualization: Enables a single physical computer to act like multiple separate computers.
- Hypervisor: The “manager” software that makes and runs the virtual computers.
- Lab Machine (VM): A whole virtual computer inside the real one, with its own system.
- Container: A small, isolated box for one app that shares the same system as the host.
- Container Images: A pre-packed recipe/template used to create containers.
- Network Ports: Special numbered entry points that apps use to talk over the network.

We also concluded that the key benefits of virtualization are:

- Cost savings
- Better resource usage
- Safe testing for cyber security
- Faster deployment
- Flexibility
- Portability
- Scalability
- Centralized Management