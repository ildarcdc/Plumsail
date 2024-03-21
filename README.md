# Plumsail
Test task for SysAdmin/DevOps

Overall architecture
   * Register an Azure instance in each region US/EU/Australia with autoscaling group and LoadBalancer (white IP)
   * Virtaualization Proxmox, if you have money I will be reserve AKS for lite management and scaling deployment and HA future
   * Register one of AZ (DevOps claster) where used Dev.steck (building, testing, deploying, logging). It is one point where connected Developers and Admins. use VPN (remoute connection)
   * This point (DevOps claster) use CI/CD for each zone have some isolated project and each project have one of administrator site
   * Сommunication between (AZ) use VPN-VPN but when expose US (AZ) use peering to communication between East and West (AZ)
   * Security of each AZ = install one instance IDS/IPS (Suricat/Fail2ban etc.) which control VPN traffic and inbound web traffic (production).
   * Regrads Ildar Issenbaeyv P.S. (It is very short description becouse there are many hidden issues in this project, needs to be discussed)
