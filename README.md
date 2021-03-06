# Container Networking Reference

A collection of tools and references around container networking accompanying my O'Reilly book _Container Networking_.

- [Networking 101](#networking-101)
- [Linux Kernel And Low-Level Components](#linux-kernel-and-low-level-components)
- [Docker](#docker)
- [Kubernetes](#kubernetes)
- [Tooling](#tooling)

![Container Networking book cover](img/cn-book.png)

---

## Networking 101

- [Network Protocols](https://www.destroyallsoftware.com/compendium/network-protocols?share_key=97d3ba4c24d21147) Programmer's Compendium
- [Demystifying container networking](http://blog.mbrt.it/2017-10-01-demystifying-container-networking/) by Michele Bertasi
- [An Empirical Study of Load Balancing Algorithms](http://liblb.com/learn.html)

## Linux Kernel And Low-Level Components

- [The History of Containers](http://red.ht/1mCDpJU)
- [A history of low-level Linux container runtimes](https://opensource.com/article/18/1/history-low-level-container-runtimes)
- [Networking in Containers and Container Clusters](http://wiki.iptables.org/pablo/netdev0.1/papers/Networking-in-Containers-and-Container-Clusters.pdf)
- [Anatomy of a Container: Namespaces, cgroups & Some Filesystem Magic](http://bit.ly/1SAn4RU) - LinuxCon
- [Network namespaces](https://lwn.net/Articles/219794/)
- [Network classifier cgroup](https://www.kernel.org/doc/Documentation/cgroup-v1/net_cls.txt)
- [Exploring LXC Networking](http://bit.ly/1kMA2hE)

## Docker

- [Docker Networking](http://bit.ly/1JXWf2R)
- [Concerning Containers’ Connections: on Docker Networking](http://bit.ly/1JXWfjl)
- [Unifying Docker Container and VM Networking](http://bit.ly/1JuCDs5)
- [Letting Go: Docker Networking and Knowing When Enough Is Enough](http://bit.ly/1TEXFVr)
- [The Tale of Two Container Networking Standards: CNM v. CNI](http://www.nuagenetworks.net/blog/container-networking-standards/)

## Kubernetes 

### Docs

- [Networking design](https://github.com/kubernetes/community/blob/master/contributors/design-proposals/network/networking.md)
- [Services](https://kubernetes.io/docs/concepts/services-networking/service/)
- [Administration—Cluster Networking](https://kubernetes.io/docs/concepts/cluster-administration/networking/)
- [Provide Load-Balanced Access to an Application in a Cluster](https://kubernetes.io/docs/tasks/access-application-cluster/load-balance-access-application-cluster/)
- [Create an External Load Balancer](https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/)
- [Kubernetes DNS example](https://github.com/kubernetes/examples/blob/master/staging/cluster-dns/README.md)
- [Issue 44063](https://github.com/kubernetes/kubernetes/issues/44063): Implement IPVS-based in-cluster service load balancing

### 3rd party

- [Data and analysis of the Kubernetes Ingress survey 2018](https://github.com/bowei/k8s-ingress-survey-2018) by the Kubernetes SIG Network
- [Kubernetes Networking 101](https://www.slideshare.net/weaveworks/kubernetes-networking-78049891) by Bryan Boreham of WeaveWorks
- [Illustrated Guide To Kubernetes Networking](https://speakerdeck.com/thockin/illustrated-guide-to-kubernetes-networking) by Tim Hockin of Google
- [The Easy--Don't Drive Yourself Crazy--Way to Kubernetes Networking](https://www.youtube.com/watch?v=H5Zl_kDOwBU) by Gerard Hickey (KubeCon 2017, Austin) 
- Blog post series by Mark Betz:
  - [Understanding kubernetes networking: pods](https://medium.com/google-cloud/understanding-kubernetes-networking-pods-7117dd28727)
  - [Understanding kubernetes networking: services](https://medium.com/google-cloud/understanding-kubernetes-networking-services-f0cb48e4cc82)
  - [Understanding kubernetes networking: ingress](https://medium.com/google-cloud/understanding-kubernetes-networking-ingress-1bc341c84078)
- [Understanding CNI (Container Networking Interface)](http://www.dasblinkenlichten.com/understanding-cni-container-networking-interface/) by Jon Langemak
- [Operating a Kubernetes network](https://jvns.ca/blog/2017/10/10/operating-a-kubernetes-network/) by Julia Evans
- [The Service Mesh: Past, Present, and Future](https://www.youtube.com/watch?v=2trOvMUuLkk) by William Morgan (KubeCon 2017, Austin)
- [Meet Bandaid, the Dropbox service proxy](https://blogs.dropbox.com/tech/2018/03/meet-bandaid-the-dropbox-service-proxy/) by Dmitry Kopytkov
- [Kubernetes NodePort vs LoadBalancer vs Ingress? When should I use what?](https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0) by Sandeep Dinesh
- [OpenShift custom router with TCP/SNI support](https://blog.zhaw.ch/icclab/openshift-custom-router-with-tcpsni-support/)

## Tooling

- [Ambassador](https://www.getambassador.io/): a Kubernetes-native API gateway built on Envoy
- [Conduit](https://conduit.io/): an ultralight service mesh for Kubernetes
- [Contour](https://github.com/heptio/contour): a Kubernetes Ingress controller for Envoy
- Kubernetes [Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/) controllers:
  - [kubernetes/ingress-gce](https://github.com/kubernetes/ingress-gce/)
  - [kubernetes/ingress-nginx](https://github.com/kubernetes/ingress-nginx)
  - [nginxinc/kubernetes-ingress](https://github.com/nginxinc/kubernetes-ingress)
  - [zlabjp/nghttpx-ingress-lb](https://github.com/zlabjp/nghttpx-ingress-lb)
- [Istio](https://istio.io/): an open platform to connect, manage, and secure microservices
- [Linkerd](https://linkerd.io/): a transparent proxy to be deployed as a service mesh
- [Træfik](https://traefik.io/): a HTTP reverse proxy and load balancer
