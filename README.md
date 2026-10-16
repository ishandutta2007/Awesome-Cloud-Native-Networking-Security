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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The cloud-native networking and security market—spanning Cloud-Native Application Protection Platforms (CNAPP), eBPF dataplanes, and multi-cloud networking—is valued at approximately **$9.4B to $14.5B** and projected to surpass **$50B+ by the early 2030s** at an estimated CAGR of **24%–28%**. The sector is **moderately to highly fragmented**, characterized by high-velocity coexistence and ongoing consolidation between hyper-scale infrastructure conglomerates (Broadcom, Cisco, IBM/Red Hat), pure-play cloud security pioneers (Palo Alto Networks, Sysdig, Aqua Security), and open-source enterprise distributions.

## SaaS/Hosted Platforms

| Platform | Company Valuation / Revenue | Starting Pricing Tier | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[VMware NSX](https://www.vmware.com/)** | **~$1.65T** (Broadcom parent market cap) | ~$90 – $115 per core/year (via VMware Cloud Foundation subscription; 16 cores/CPU minimum) | **60-day free evaluation** (enterprise trial with full feature access via Broadcom portal) | Enterprise network virtualization and security platform with container networking via NSX Container Plugin (NCP) for vSphere & Tanzu. |
| **[Isovalent Enterprise Cilium (Cisco)](https://isovalent.com/)** | **~$430B** (Cisco parent market cap; acquired for ~$650M) | ~$600 per node/year (Enterprise Essentials tier, annual commit) | **Free interactive sandbox labs** (guided browser sessions at isovalent.com/labs with no cluster limits; custom 30-day enterprise PoC on request) | Enterprise version of Cilium with troubleshooting, operational support, multi-cluster Cluster Mesh, and commercial eBPF networking. |
| **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** | **~$310B** (Market Cap) | ~$18,000/year (or ~$1.20 per credit; 2 credits/VM for Foundations, 5 credits/VM for Advanced) | **30-day free trial** (access to CSPM, CWPP, and code security modules without upfront credit card commitment) | Comprehensive CNAPP platform offering CWPP, CSPM, CIEM, WAAS, and code-to-cloud security across multi-cloud environments. |
| **[Red Hat Advanced Cluster Security (StackRox)](https://www.redhat.com/en/technologies/cloud-computing/openshift/advanced-cluster-security-kubernetes)** | **~$212B** (IBM parent market cap; acquired Red Hat for $34B) | ~$0.028 per vCPU/hour on-demand (RHACS Cloud Service via AWS Marketplace) | **60-day free trial** (self-supported trial limited to 20 cores or 80 vCPUs across Kubernetes/OpenShift clusters) | Kubernetes-native security platform featuring vulnerability management, network segmentation, risk profiling, and compliance reporting. |
| **[Dynatrace](https://www.dynatrace.com/)** | **~$18.5B** (Market Cap) | $0.00225 per memory-GiB-hour (~$13/month per 8 GiB host for Application Security) | **15-day free trial** (includes full-stack observability and runtime vulnerability analytics) | Unified observability platform featuring runtime Kubernetes vulnerability analytics, threat detection, and automated remediation. |
| **[NeuVector (SUSE)](https://neuvector.com/)** | **~$6.0B** (SUSE private equity valuation) | ~$112 per node/month (AWS Marketplace pay-as-you-go; 5–15 nodes bracket) | **Free forever open-source edition** (full Layer 7 container firewall on GitHub with no node limits; commercial NeuVector Prime features a 30-day eval) | Full lifecycle container security platform featuring Layer 7 container firewall, deep packet inspection, and process profiling. |
| **[Sysdig Secure](https://sysdig.com/)** | **~$2.5B** (Valuation at Series G) | $72 per host/month (CNAPP Enterprise tier, 20-host minimum commitment) | **30-day free trial** (full runtime threat detection, Falco rules engine, and CSPM features) | Cloud-native security platform with deep runtime threat detection, vulnerability management, and forensics powered by Falco. |
| **[Aqua Security](https://www.aquasec.com/)** | **~$1.0B+** (Valuation at Series E) | ~$35 – $55 per workload/month (Enterprise list price; or ~$10,000/year entry package) | **14-day free trial** (full CNAPP workload protection evaluation; unlimited free open-source scanner via Trivy) | Cloud-native security platform covering vulnerability scanning, container runtime protection, secrets management, and compliance. |
| **[Tigera Calico Enterprise](https://www.tigera.io/)** | **~$250M – $350M** (Estimated; $53M total VC funding raised) | $0.025 per vCPU/hour (Calico Cloud consumption billing via AWS/Azure Marketplace) | **Free forever plan** (strictly 1 connected Kubernetes cluster running Calico OSS 3.30+, includes 24-hr flow log retention and service graph) | Self-managed and SaaS platform for Kubernetes networking, hierarchical tiered network policies, SIEM integrations, and workload-centric WAF. |



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
