# Network namespaces

Network namespaces in Linux provide a way to **isolate network resources and configurations at the kernel level**.

They allow you to create multiple independent network stacks within a single Linux system, effectively creating isolated network environments.

To create a network namespace:

`sudo ip netns add my-virtual-namespace`

To display the created network namespace:

`sudo ip netns show my-virtual-namespace`

# Virtual network interfaces

- Linux provides a way to create virtual network inside a host
- Virtual network interfaces are conceptually same thing as ethernet interface provided by a physical network interface card (NIC) but are virtualized
- Since it's same like a real world ethernet interface, it can have a virtual MAC address as well
- Using virtual network interfaces, we can create a virtual ethernet pair which consists of two ends (veth0 and veth1) that are connected to each other
  - The veth pair serves as a communication channel, allowing data to be transmitted between the virtualized environment and the host

To Create a virtual ethernet pair:

`sudo ip link add veth0 type veth peer name veth1`

To display MAC address of the created veth pair:

`sudo ip link show veth0`

`sudo ip link show veth1`
