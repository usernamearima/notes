# Virtualization Basics

These notes cover the fundamentals of virtualization.
Virtualization is a core concept in cybersecurity labs,
cloud computing, malware analysis, and testing environments.

---

## 1. What Is Virtualization

Virtualization allows running multiple operating systems
on a single physical machine.

Each operating system runs in an isolated environment
called a virtual machine (VM).

The physical machine is called the host.
The virtual machines are called guests.

---

## 2. Why Virtualization Is Used

Virtualization is used to:
- save hardware resources
- isolate systems
- test software safely
- create lab environments
- simulate networks

In cybersecurity, virtualization is essential
for safe experimentation.

---

## 3. Virtual Machine (VM)

A virtual machine behaves like a real computer.

A VM has:
- its own operating system
- virtual CPU
- virtual memory (RAM)
- virtual disk
- virtual network interface

From inside the VM,
it looks like a normal computer.

---

## 4. Hypervisor

A hypervisor is software that creates and manages virtual machines.

The hypervisor:
- allocates hardware resources
- isolates virtual machines
- controls VM lifecycle

---

## 5. Types of Hypervisors

### Type 1 – Bare Metal
Runs directly on hardware.

Characteristics:
- high performance
- used in servers and data centers

Examples:
- VMware ESXi
- Hyper-V Server

---

### Type 2 – Hosted
Runs on top of a host operating system.

Characteristics:
- easier to use
- common on personal computers

Examples:
- VirtualBox
- VMware Workstation

---

## 6. Snapshots

A snapshot is a saved state of a virtual machine.

Snapshots allow you to:
- revert changes
- recover from mistakes
- test risky actions safely

Snapshots are heavily used in:
- malware analysis
- security labs
- system testing

---

## 7. Virtual Networking

Virtual machines can have different network configurations.

Common modes:
- NAT – VM accesses the internet through the host
- Bridged – VM appears as a separate device on the network
- Host-only – VM communicates only with the host

Network mode selection affects:
- isolation
- visibility
- attack surface

---

## 8. Isolation and Security

Virtual machines are isolated from:
- each other
- the host system

Isolation helps:
- limit damage
- contain malware
- test attacks safely

However:
- misconfiguration can break isolation
- shared folders and devices increase risk

---

## 9. Virtualization in Cybersecurity

Virtualization is used for:
- penetration testing labs
- malware analysis
- exploit testing
- incident response training
- blue team simulations

Most learning environments rely on virtualization.

---

## 10. Limitations of Virtualization

Virtualization is not perfect.

Limitations include:
- performance overhead
- detection by malware
- misconfiguration risks

Virtual machines improve safety,
but they do not guarantee full security.

---

## Key Takeaways

- virtualization runs multiple systems on one machine
- virtual machines are isolated environments
- hypervisors manage virtual machines
- snapshots enable safe rollback
- virtual networking controls connectivity
- virtualization is critical for cybersecurity labs
