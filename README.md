# Awesome-Cloud-Native-Networking-Security

# Awesome-Cloud-Native-Networking-Security

## Top Cloud-Native Networking & Security Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on eBPF Dataplanes, Runtime Security & Kubernetes-Native Threat Detection*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud-Native Networking & Security**. These tools enable organizations to provide pod connectivity, enforce network policies, and gain deep runtime security into cluster workloads—from eBPF-based dataplanes that bypass kube-proxy to container runtime security that detects threats in real time.



**Examples** include Cilium, Isovalent Enterprise, Tigera Calico, VMware NSX, Red Hat Advanced Cluster Security, Aqua Security, Sysdig Secure, Palo Alto Prisma Cloud, NeuVector, and Dynatrace (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, eBPF-based networking, and open runtime security—ideal for platform engineers, security teams, and organizations seeking transparent, vendor-independent cloud-native security.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Isovalent Enterprise Cilium (Cisco)](https://isovalent.com/)**  

  **Enterprise version of Cilium with troubleshooting, operational support, and multi-cluster capabilities** . **Cluster Mesh** enables **failover to other clusters** when resources become unavailable or misconfigured . **Cisco acquired Isovalent** in 2024, integrating Cilium into Cisco's multicloud networking portfolio . **The most mature commercial eBPF networking platform** .



- **[Tigera Calico Enterprise](https://www.tigera.io/)**  

  **Self-managed platform for Kubernetes networking, network security, and observability** . **Extends Calico Open Source** with **hierarchical tiered network policy**, **DNS/FQDN-based policy**, **policy recommendations**, **SIEM integrations**, **workload-centric WAF**, and **compliance reporting** . **Calico Cloud Free Tier** provides **observability and policy management for a single cluster** at no cost . **The enterprise standard** for organizations requiring regulatory compliance.



- **[VMware NSX](https://www.vmware.com/)**  

  **Enterprise network virtualization and security platform** with container networking via **NSX Container Plugin (NCP)** . **The most integrated with VMware ecosystem** for organizations running vSphere and Tanzu.



- **[Red Hat Advanced Cluster Security (StackRox)](https://www.redhat.com/en/technologies/cloud-computing/openshift/advanced-cluster-security-kubernetes)**  

  **Kubernetes-native security platform** (built on StackRox OSS) . Features **vulnerability management**, **configuration management**, **network segmentation**, **risk profiling**, **threat detection**, and **compliance reporting** . **The standard for OpenShift security** .



- **[Aqua Security](https://www.aquasec.com/)**  

  **Cloud-native security platform** with **vulnerability scanning**, **runtime protection**, **secrets management**, and **compliance** . **The most comprehensive CNAPP** for container and cloud workloads .



- **[Sysdig Secure](https://sysdig.com/)**  

  **Cloud-native security with runtime insights** powered by **Falco** (which Sysdig created) . Features **threat detection**, **vulnerability management**, **compliance**, and **forensics** . **The most runtime-focused commercial platform** .



- **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)**  

  **Comprehensive CNAPP** with **CWPP, CSPM, CIEM, and code security** . **The most comprehensive enterprise platform** for multi-cloud security .



- **[NeuVector (SUSE)](https://neuvector.com/)**  

  **Full lifecycle container security platform**—**the only open-source solution with Layer 7 container firewall** . Features **deep packet inspection**, **process profiling**, **DLP**, and **admission control** . **The most security-focused open-source container platform** .



- **[Dynatrace](https://www.dynatrace.com/)**  

  **Observability platform with Kubernetes security** . Features **runtime vulnerability analytics**, **threat detection**, and **automated remediation** .



## Open-Source GitHub Projects



- **[Calico Open Source](https://github.com/projectcalico/calico)**  

  **Cloud native networking and network security** (Apache-2.0) . **The most widely used container networking solution**—supports **Kubernetes, OpenShift, OpenStack, and bare metal** . **Core capabilities**: **high-performance pod networking**, **advanced IP address management**, **seamless Kubernetes NetworkPolicy support**, **global default deny policy**, **DNS/FQDN-based policy**, **data-in-transit encryption via WireGuard**, and **multiple dataplane options** (eBPF, iptables, nftables, Windows HNS, VPP) . **Calico's encryption performance is notable**: benchmark testing shows **Calico TCP bandwidth at 9,786 Mbit/s under encryption versus Cilium's 1,386 Mbit/s**—approximately **7x higher throughput** . **The enterprise-grade choice** for organizations requiring BGP peering with physical networks and strict policy enforcement .



- **[Cilium](https://github.com/cilium/cilium)**  

  **eBPF-based Networking, Security, and Observability** (Apache-2.0) . **The de facto standard for cloud-native networking**—**over 60% of CNI deployments** according to the State of Kubernetes Networking report, **more than double the next alternative** . **24,000+ GitHub stars** and **1,010+ developers** . **Core capabilities**: **identity-based NetworkPolicy** enforcement at L3/L4, **L7 policy** for HTTP/gRPC/Kafka, **ClusterIP load-balancing via eBPF** (bypassing kube-proxy), and **mutual authentication with ztunnel** . **Hubble** provides **fully distributed networking and security observability**—answering "which services experienced DNS resolution problems?", "what is the 99th percentile latency?", and "which connections were blocked by policy?" . **Adopted by all major cloud providers** including GKE Dataplane V2, Azure Kubernetes Service, and OVHcloud's Managed Kubernetes Service . **The reference implementation for eBPF-based Kubernetes networking** .



- **[Falco](https://github.com/falcosecurity/falco)**  

  **Cloud-native runtime security** (Apache-2.0) . **The de facto standard for runtime threat detection**—**CNCF Graduated project** with **1M+ downloads** and **100+ contributors** . **Uses syscall and eBPF instrumentation** to detect anomalous activity, container escapes, privilege escalation, and file access violations in real time . **Feature-rich rule engine** with **out-of-the-box rules** for MITRE ATT&CK techniques . **Kubernetes audit log support** through the Kubernetes Audit Events plugin . **The foundation for Sysdig Secure and many commercial platforms** . **The reference implementation for runtime security on Linux and Kubernetes** .



- **[Tetragon](https://github.com/cilium/tetragon)**  

  **eBPF-based Security Observability and Runtime Enforcement** (Apache-2.0) . **The emerging standard for eBPF-native runtime security** from the Cilium project . **Provides deep visibility into process execution, network activity, and file access** with **eBPF enforcement capabilities** . **Combines with Cilium** for a complete eBPF networking and security stack . **The most modern open-source runtime security tool** .



- **[KubeArmor](https://github.com/kubearmor/KubeArmor)**  

  **Cloud-native runtime security enforcement system** (Apache-2.0) . **The most comprehensive open-source runtime security platform**—**works at the kernel level** (LSM-based) to restrict process execution, file access, and network operations . **Supports AppArmor, SELinux, and BPF-LSM** . **The CNCF sandbox project** for workload hardening .



- **[Kyverno](https://github.com/kyverno/kyverno)**  

  **Kubernetes-native policy management** (Apache-2.0) . **The standard for admission control policies**—**validates, mutates, and generates Kubernetes resources** using policies written as Kubernetes resources . **CNCF Incubating project** with **7,000+ GitHub stars** . **The simplest policy engine for Kubernetes**—no new language to learn .



- **[Open Policy Agent (OPA)](https://github.com/open-policy-agent/opa)**  

  **Open-source, general-purpose policy engine** (Apache-2.0) . **The standard for policy-as-code**—**CNCF Graduated project** with **9,000+ GitHub stars** . **Used by Kubernetes admission control (via Gatekeeper), CI/CD pipelines, API gateways, and microservices** . **Rego language** for policy expression . **The most widely deployed policy engine** in cloud-native infrastructure .



- **[Gatekeeper](https://github.com/open-policy-agent/gatekeeper)**  

  **Kubernetes admission controller that enforces policies using OPA** (Apache-2.0) . **The standard for OPA-based Kubernetes policy enforcement** . **Combines with Kyverno** for comprehensive policy coverage .



- **[Trivy](https://github.com/aquasecurity/trivy)**  

  **Comprehensive security scanner for vulnerabilities, misconfigurations, secrets, and SBOMs** (Apache-2.0) . **The most widely used open-source vulnerability scanner**—**25,000+ GitHub stars** . **Scans container images, filesystems, Git repositories, Kubernetes clusters, and IaC** . **The default scanner for many CI/CD pipelines** .



- **[Kubescape](https://github.com/kubescape/kubescape)**  

  **Kubernetes security posture management** (Apache-2.0) . **The most comprehensive open-source KSPM**—**scans clusters against NSA/CISA, MITRE ATT&CK, and SOC 2 frameworks** . **Features**: **risk analysis**, **security posture scoring**, **RBAC visualization**, **network policy generation**, and **CI/CD integration** .



- **[Kube-bench](https://github.com/aquasecurity/kube-bench)**  

  **Checks Kubernetes against CIS Benchmark** (Apache-2.0) . **The standard for Kubernetes hardening**—**runs checks against control plane, worker nodes, and policies** . **The default for compliance validation** .



### Additional Strong Open-Source Options



- **[Hubble](https://github.com/cilium/hubble)** — Fully distributed networking and security observability platform (Apache-2.0) . **The standard for CNI-level observability**—answers DNS, latency, and policy-blocked connection queries .

- **[StackRox](https://github.com/stackrox/stackrox)** — Kubernetes-native security platform (Apache-2.0) . **The open-source foundation for Red Hat Advanced Cluster Security** .

- **[Kube-hunter](https://github.com/aquasecurity/kube-hunter)** — Kubernetes penetration testing tool (Apache-2.0) . **The standard for offensive security validation** .

- **[Trivy Operator](https://github.com/aquasecurity/trivy-operator)** — Kubernetes-native security toolkit (Apache-2.0) . **The standard for continuous vulnerability scanning in clusters** .

- **[KubeLinter](https://github.com/stackrox/kube-linter)** — Static analysis for Kubernetes YAML files and Helm charts (Apache-2.0) . **The standard for manifest linting** .

- **[Polaris](https://github.com/FairwindsOps/polaris)** — Kubernetes configuration validation (Apache-2.0) . **The standard for workload best-practice checks** .

- Community **n8n** workflows for security alert routing and compliance evidence automation.



**Frameworks for building custom systems**: Combine **Cilium** for eBPF-native networking and observability with **Tetragon** for runtime enforcement, **Falco** for threat detection, **OPA/Gatekeeper** for admission policy, **Trivy** for vulnerability scanning, and **Kubescape** for posture management—creating a fully self-hosted, enterprise-grade cloud-native security platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud-native security tools handling cluster traffic and workload data must follow security best practices and implement appropriate access controls.

- **Open-source cloud-native security is mature and production-ready.** Cilium represents **over 60% of CNI deployments** . Falco is the **de facto standard for runtime threat detection**—CNCF Graduated with 1M+ downloads . OPA is the **standard for policy-as-code** . **These are genuine alternatives to commercial platforms.**

- **Cilium vs Calico: the choice depends on your priorities.** Cilium offers **eBPF-native performance**, **L7 policy**, and **Hubble observability**—ideal for cloud-native, microservices-heavy environments . Calico offers **mature BGP peering**, **broader dataplane options**, and **significantly better encryption throughput** (9,786 vs 1,386 Mbit/s in benchmark testing) . **Cilium for observability and L7 policy; Calico for bare-metal BGP and encryption-heavy workloads** .

- **Runtime security requires layered defense.** Falco detects threats via syscall monitoring . Tetragon enforces via eBPF . KubeArmor restricts via LSM (AppArmor, SELinux, BPF-LSM) . **No single tool covers all runtime security needs**—combine detection, enforcement, and hardening.

- **Policy-as-code is the governance layer.** OPA and Gatekeeper provide admission control . Kyverno provides Kubernetes-native policy management without a new language . **The right choice depends on whether your team prefers Rego or Kubernetes-native YAML.**

- Self-hosted open-source solutions require proper kernel compatibility (eBPF requires Linux 5.4+, recommended 5.10+), CNI configuration, and ongoing maintenance. **Network policies are your primary security boundary**—default-deny is the recommended starting posture.



---



**Made for platform engineers, security teams, and organizations building transparent cloud-native security solutions.**  

Let's make Cloud-Native Networking & Security more open, data-driven, and observable.
