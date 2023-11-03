# Glimps of underlying Technology for `docker`

## Linux Containers (LXC)
- **Linux Containers** serve as the foundation for _Docker_.


## Control Groups (cgroups)
- A _control groups_ is a Linux kernel feature that limits, accounts for, and isolates the resource usage(CPU, memory, disk I/O, network, and so on) of a collection of process.
- It provides below features.
    1. **Resource limits** : You can configure a cgroup to limit how much of a particular resource a process can use.
    2. **Prioritization** : You can control how much of a resource a process can use compared to processes in another cgroup when there is resource contention.
    3. **Accounting** : Resouce limits are monitored and reported at the cgroup level.
    4. **Control** : You can change the status(frozen, stopped, or restarted) of all processes in a cgroup with a single command.

- [Resouce](https://www.nginx.com/blog/what-are-namespaces-cgroups-how-do-they-work/)


## Union file Systems (UnionFS)
- UnionFS is a file system service that allows the overlaying of multiple file systems in a single, unified view.
- Docker uses UnionFS to create a layered approach for _images_ and _containers_, which enables better sharing of common files and faster container creation. 


## Namespaces
- **Namespaces** are another _Linux kernel_ feature that provides process isolation.
- The allow *Docker* to create isolated workspaces called containers.
- It ensure that process within container cannot interfere with process outside the container or on the host system.
- There are several types of namespaces, like PID, NET, MNT and USER, each responsible for isolating a different aspect of a process.