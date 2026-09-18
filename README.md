# R2: portable device for auditing and diagnosis of Linux server

R2 is an academic project to design and implement a portable, autonomous device for
the controlled auditing and diagnosis of Linux servers and infrastructures. The device
will use a single-board computer with network connectivity and a screen to present the
audit status and summarized results.

The audit combines two perspectives:

- **External analysis:** checking which services, ports, and configurations are actually
  accessible over the network.
- **Internal analysis:** connecting through authorized SSH access to inspect users,
  services, permissions, firewall rules, updates, storage, and system configuration.

Comparing both perspectives should reveal discrepancies between a server's internal
configuration and its externally exposed state, without installing permanent agents on
the audited systems. Planned extensions include comparing audits over time, sending
results to a central server for history, and signing reports to protect their integrity
and authenticity.

Development will proceed incrementally, beginning with software and virtual-machine
laboratories, followed by external auditing and result comparison, report generation,
and finally deployment on a Linux-configured single-board computer with a display and,
if needed, physical selection buttons. The finished system will be evaluated in
controlled scenarios using detection capability, false positives, execution time,
server load, and behavior across different configurations.
