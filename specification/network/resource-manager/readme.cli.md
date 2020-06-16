## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  cli-name: network
  package-name: azure-mgmt-network
  namespace: azure.mgmt.network
  test-scenario:
    - split: publicipaddresses
    - name: /PublicIPAddresses/put/Create public IP address DNS
    - name: /PublicIPAddresses/put/Create public IP address allocation method
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /PublicIPAddresses/get/GetVMSSPublicIP
    - name: /PublicIPAddresses/get/ListVMSSVMPublicIP
    - name: /PublicIPAddresses/get/ListVMSSPublicIP
    - name: /PublicIPAddresses/get/Get public IP address
    - name: /PublicIPAddresses/get/List resource group public IP addresses
    - name: /PublicIPAddresses/get/List all public IP addresses
    - name: /PublicIPAddresses/patch/Update public IP address tags
    - name: /PublicIPAddresses/delete/Delete public IP address
    - split: virtualnetworks
    - name: /VirtualNetworks/put/Create virtual network with service endpoints and service endpoint policy
    - name: /VirtualNetworks/put/Create virtual network with subnet containing address prefixes
    - name: /VirtualNetworks/put/Create virtual network with Bgp Communities
    - name: /VirtualNetworks/put/Create virtual network
    - name: /VirtualNetworks/put/Create virtual network with service endpoints
    - name: /VirtualNetworks/put/Create virtual network with subnet
    - name: /VirtualNetworks/put/Create virtual network with delegated subnets
    - name: /VirtualNetworks/get/Check IP address availability
    - name: /VirtualNetworks/get/VnetGetUsage
    - name: /VirtualNetworks/get/Get virtual network
    - name: /VirtualNetworks/get/Get virtual network with service association links
    - name: /VirtualNetworks/get/Get virtual network with a delegated subnet
    - name: /VirtualNetworks/get/List virtual networks in resource group
    - name: /VirtualNetworks/get/List all virtual networks
    - name: /VirtualNetworks/patch/Update virtual network tags
    - name: /VirtualNetworks/delete/Delete virtual network
    - split: subnets
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /Subnets/put/Create subnet with service endpoints
    - name: /Subnets/put/Create subnet with a delegation
    - name: /Subnets/get/Get subnet with a delegation
    - name: /Subnets/get/Get subnet
    - name: /Subnets/get/List subnets
    - name: /Subnets/post/Unprepare Network Policies
      comment: "Azure Error: UnauthorizedOperation"
      disabled: true
    - name: /Subnets/post/Prepare Network Policies
      comment: "Azure Error: UnauthorizedOperation"
      disabled: true
    - name: /Subnets/delete/Delete subnet
    - split: loadbalancers
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /LoadBalancers/put/Create load balancer with Frontend IP in Zone 1
    - name: /LoadBalancers/put/Create load balancer with outbound rules
    - name: /LoadBalancers/put/Create load balancer with Standard SKU
    - name: /LoadBalancers/put/Create load balancer
    - name: /LoadBalancers/put/Create load balancer with inbound nat pool
    - name: /LoadBalancers/get/Get load balancer
    - name: /LoadBalancers/get/List load balancers in resource group
    - name: /LoadBalancers/get/List all load balancers
    - name: /LoadBalancers/patch/Update load balancer tags
    - name: /LoadBalancers/delete/Delete load balancer
    - split: networkinterfaces
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /NetworkInterfaces/put/Create network interface
    - name: /NetworkInterfaces/get/Get virtual machine scale set network interface
    - name: /NetworkInterfaces/get/List virtual machine scale set network interface ip configurations
    - name: /NetworkInterfaces/get/Get virtual machine scale set network interface
    - name: /NetworkInterfaces/get/List virtual machine scale set vm network interfaces
    - name: /NetworkInterfaces/get/List virtual machine scale set network interfaces
    - name: /NetworkInterfaces/get/Get network interface
    - name: /NetworkInterfaces/get/List network interfaces in resource group
    - name: /NetworkInterfaces/get/List all network interfaces
    - name: /NetworkInterfaces/post/List network interface effective network security groups
    - name: /NetworkInterfaces/post/Show network interface effective route tables
    - name: /NetworkInterfaces/patch/Update network interface tags
    - name: /NetworkInterfaces/delete/Delete network interface
    - split: routetables
    - name: /RouteTables/put/Create route table with route
    - name: /RouteTables/put/Create route table
    - name: /RouteTables/get/Get route table
    - name: /RouteTables/get/List route tables in resource group
    - name: /RouteTables/get/List all route tables
    - name: /RouteTables/patch/Update route table tags
    - name: /RouteTables/delete/Delete route table
    - split: routes
    - name: /RouteTables/put/Create route table
    - name: /Routes/put/Create route
    - name: /Routes/get/Get route
    - name: /Routes/get/List routes
    - name: /Routes/delete/Delete route
    - split: routefilters
    - name: /RouteFilters/put/RouteFilterCreate
    - name: /RouteFilters/get/RouteFilterGet
    - name: /RouteFilters/get/RouteFilterListByResourceGroup
    - name: /RouteFilters/get/RouteFilterList
    - name: /RouteFilters/patch/Update route filter tags
    - name: /RouteFilters/delete/RouteFilterDelete
    - split: routefilterrules
    - name: /RouteFilters/put/RouteFilterCreate
    - name: /RouteFilterRules/put/RouteFilterRuleCreate
    - name: /RouteFilterRules/get/RouteFilterRuleGet
    - name: /RouteFilterRules/get/RouteFilterRuleListByRouteFilter
    - name: /RouteFilterRules/delete/RouteFilterRuleDelete
    - split: virtualwans
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualWans/get/VirtualWANGet
    - name: /VirtualWans/get/VirtualWANListByResourceGroup
    - name: /VirtualWans/get/VirtualWANList
    - name: /VirtualWans/patch/VirtualWANUpdate
    - name: /VirtualWans/delete/VirtualWANDelete
    - split: virtualhubs
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /VirtualHubs/get/VirtualHubGet
    - name: /VirtualHubs/get/VirtualHubListByResourceGroup
    - name: /VirtualHubs/get/VirtualHubList
    - name: /VirtualHubs/patch/VirtualHubUpdate
    - name: /VirtualHubs/delete/VirtualHubDelete
    - split: virtualhubroutetablev2s
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /VirtualHubRouteTableV2s/put/VirtualHubRouteTableV2Put
    - name: /VirtualHubRouteTableV2s/get/VirtualHubVirtualHubRouteTableV2Get
    - name: /VirtualHubRouteTableV2s/get/VirtualHubRouteTableV2List
    - name: /VirtualHubRouteTableV2s/delete/VirtualHubRouteTableV2Delete
    - split: vpnsites
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VpnSites/put/VpnSiteCreate
    - name: /VpnSites/get/VpnSiteGet
    - name: /VpnSites/get/VpnSiteListByResourceGroup
    - name: /VpnSites/get/VpnSiteList
    - name: /VpnSites/patch/VpnSiteUpdate
    - name: /VpnSites/delete/VpnSiteDelete
    - split: ipgroups
    - name: /IpGroups/put/CreateOrUpdate_IpGroups
    - name: /IpGroups/get/Get_IpGroups
    - name: /IpGroups/get/ListByResourceGroup_IpGroups
    - name: /IpGroups/get/List_IpGroups
    - name: /IpGroups/patch/Update_IpGroups
      comment: The requested resource does not support http method 'PATCH'.
      disabled: true
    - name: /IpGroups/delete/Delete_IpGroups
    - split: bastionhosts
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /BastionHosts/put/Create Bastion Host
    - name: /BastionHosts/get/Get Bastion Host
    - name: /BastionHosts/get/List all Bastion Hosts for a given resource group
    - name: /BastionHosts/get/List all Bastion Hosts for a given subscription
    - name: /BastionHosts/delete/Delete Bastion Host
    - split: inboundnatrules
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /LoadBalancers/put/Create load balancer
    - name: /InboundNatRules/put/InboundNatRuleCreate
    - name: /InboundNatRules/get/InboundNatRuleGet
    - name: /InboundNatRules/get/InboundNatRuleList
    - name: /InboundNatRules/delete/InboundNatRuleDelete
    - split: networksecuritygroups
    - name: /NetworkSecurityGroups/put/Create network security group
    - name: /NetworkSecurityGroups/put/Create network security group with rule
    - name: /NetworkSecurityGroups/get/Get network security group
    - name: /NetworkSecurityGroups/get/List network security groups in resource group
    - name: /NetworkSecurityGroups/get/List all network security groups
    - name: /NetworkSecurityGroups/patch/Update network security group tags
    - name: /NetworkSecurityGroups/delete/Delete network security group
    - split: securityrules
    - name: /NetworkSecurityGroups/put/Create network security group
    - name: /SecurityRules/put/Create security rule
    - name: /SecurityRules/get/List network security rules in network security group
    - name: /SecurityRules/get/Get network security rule in network security group
    - name: /SecurityRules/delete/Delete network security rule from network security group
    - split: ipallocations
    - name: /VirtualNetworks/put/Create virtual network
    - name: /IpAllocations/put/Create IpAllocation
      comment: "Azure Error: HypernetIpAllocationSubscriptionNotOnboardHypernet"
    - name: /IpAllocations/get/Get IpAllocation
    - name: /IpAllocations/get/List IpAllocations in resource group
    - name: /IpAllocations/get/List all IpAllocations
    - name: /IpAllocations/patch/Update virtual network tags
    - name: /IpAllocations/delete/Delete IpAllocation
    - split: publicipprefixes
    - name: /PublicIPPrefixes/put/Create public IP prefix defaults
    - name: /PublicIPPrefixes/put/Create public IP prefix allocation method
    - name: /PublicIPPrefixes/get/Get public IP prefix
    - name: /PublicIPPrefixes/get/List resource group public IP prefixes
    - name: /PublicIPPrefixes/get/List all public IP prefixes
    - name: /PublicIPPrefixes/patch/Update public IP prefix tags
    - name: /PublicIPPrefixes/delete/Delete public IP prefix
    - split: firewallpolicies
    - name: /IpGroups/put/CreateOrUpdate_IpGroups
    - name: /FirewallPolicies/put/Create FirewallPolicy
    - name: /FirewallPolicyRuleGroups/put/Create FirewallPolicyRuleGroup
    - name: /FirewallPolicyRuleGroups/put/Create FirewallPolicyRuleGroup With IpGroups
      disabled: true
      comment: Need to construct test with two IP Groups
    - name: /FirewallPolicyRuleGroups/get/Get FirewallPolicyRuleGroup With IpGroups
      disabled: true
      comment: Need to construct test with two IP Groups
    - name: /FirewallPolicyRuleGroups/get/Get FirewallPolicyRuleGroup
    - name: /FirewallPolicyRuleGroups/get/List all FirewallPolicyRuleGroups for a given FirewallPolicy
    - name: /FirewallPolicyRuleGroups/get/List all FirewallPolicyRuleGroups with IpGroups for a given FirewallPolicy
    - name: /FirewallPolicies/get/Get FirewallPolicy
    - name: /FirewallPolicies/get/List all Firewall Policies for a given resource group
    - name: /FirewallPolicies/get/List all Firewall Policies for a given subscription
    - name: /FirewallPolicyRuleGroups/delete/Delete FirewallPolicyRuleGroup
    - name: /FirewallPolicies/delete/Delete Firewall Policy
    - split: virtualrouters
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /VirtualNetworkGateways/put/UpdateVirtualNetworkGateway
    - name: /VirtualRouters/put/Create VirtualRouter
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouters/get/Get VirtualRouter
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouters/get/List all Virtual Router for a given resource group
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouters/get/List all Virtual Routers for a given subscription
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouters/delete/Delete VirtualRouter
      disabled: true
      comment: This feature is not enabled
    - split: azurefirewalls
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /AzureFirewalls/put/Create Azure Firewall With IpGroups
    - name: /AzureFirewalls/put/Create Azure Firewall With Additional Properties
    - name: /AzureFirewalls/put/Create Azure Firewall in virtual Hub
    - name: /AzureFirewalls/put/Create Azure Firewall With management subnet
    - name: /AzureFirewalls/put/Create Azure Firewall With Zones
    - name: /AzureFirewalls/put/Create Azure Firewall
    - name: /AzureFirewalls/get/Get Azure Firewall
    - name: /AzureFirewalls/get/Get Azure Firewall With Zones
    - name: /AzureFirewalls/get/Get Azure Firewall With management subnet
    - name: /AzureFirewalls/get/Get Azure Firewall With Additional Properties
    - name: /AzureFirewalls/get/Get Azure Firewall With IpGroups
    - name: /AzureFirewalls/get/List all Azure Firewalls for a given resource group
    - name: /AzureFirewalls/get/List all Azure Firewalls for a given subscription
    - name: /AzureFirewalls/patch/Update Azure Firewall Tags
    - name: /AzureFirewalls/delete/Delete Azure Firewall
    - split: vpngateways
    - name: /VpnGateways/put/VpnGatewayPut
    - name: /VpnGateways/get/VpnGatewayGet
    - name: /VpnGateways/get/VpnGatewayListByResourceGroup
    - name: /VpnGateways/get/VpnGatewayListBySubscription
    - name: /VpnGateways/post/ResetVpnGateway
    - name: /VpnGateways/patch/VpnGatewayUpdate
    - name: /VpnGateways/delete/VpnGatewayDelete
    - split: natgateways
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /PublicIPPrefixes/put/Create public IP prefix defaults
    - name: /NatGateways/put/Create nat gateway
    - name: /NatGateways/get/Get nat gateway
    - name: /NatGateways/get/List nat gateways in resource group
    - name: /NatGateways/get/List all nat gateways
    - name: /NatGateways/patch/Update nat gateway tags
    - name: /NatGateways/delete/Delete nat gateway
    - split: virtualnetworktaps
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /NetworkInterfaces/put/Create network interface
    - name: /VirtualNetworkTaps/put/Create Virtual Network Tap
    - name: /VirtualNetworkTaps/get/Get Virtual Network Tap
    - name: /VirtualNetworkTaps/get/List virtual network taps in resource group
    - name: /VirtualNetworkTaps/get/List all virtual network taps
    - name: /VirtualNetworkTaps/patch/Update virtual network tap tags
    - name: /VirtualNetworkTaps/delete/Delete Virtual Network Tap resource
    - split: networkinterfacetapconfigurations
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /NetworkInterfaces/put/Create network interface
    - name: /VirtualNetworkTaps/put/Create Virtual Network Tap
    - name: /NetworkInterfaceTapConfigurations/put/Create Network Interface Tap Configurations
    - name: /NetworkInterfaceTapConfigurations/get/Get Network Interface Tap Configurations
    - name: /NetworkInterfaceTapConfigurations/get/List virtual network tap configurations
    - name: /NetworkInterfaceTapConfigurations/delete/Delete tap configuration
    - split: virtualnetworkgateways
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /VirtualNetworkGateways/put/UpdateVirtualNetworkGateway
    - name: /VirtualNetworkGateways/get/VirtualNetworkGatewaysListConnections
    - name: /VirtualNetworkGateways/get/GetVirtualNetworkGateway
    - name: /VirtualNetworkGateways/get/ListVirtualNetworkGatewaysinResourceGroup
    - name: /VirtualNetworkGateways/post/Disconnect VpnConnections from Virtual Network Gateway
    - name: /VirtualNetworkGateways/post/GetVPNDeviceConfigurationScript
    - name: /VirtualNetworkGateways/post/GetVirtualNetworkGatewayVpnclientConnectionHealth
    - name: /VirtualNetworkGateways/post/Set VirtualNetworkGateway VpnClientIpsecParameters
    - name: /VirtualNetworkGateways/post/Get VirtualNetworkGateway VpnClientIpsecParameters
    - name: /VirtualNetworkGateways/post/GenerateVPNClientPackage
    - name: /VirtualNetworkGateways/post/GetVirtualNetworkGatewayVPNProfilePackageURL
    - name: /VirtualNetworkGateways/post/ResetVpnClientSharedKey
    - name: /VirtualNetworkGateways/post/ListVirtualNetworkGatewaySupportedVPNDevices
    - name: /VirtualNetworkGateways/post/GetVirtualNetworkGatewayAdvertisedRoutes
    - name: /VirtualNetworkGateways/post/Start packet capture on virtual network gateway without filter
    - name: /VirtualNetworkGateways/post/Start packet capture on virtual network gateway with filter
    - name: /VirtualNetworkGateways/post/GenerateVirtualNetworkGatewayVPNProfile
    - name: /VirtualNetworkGateways/post/Stop packet capture on virtual network gateway
    - name: /VirtualNetworkGateways/post/GetVirtualNetworkGatewayLearnedRoutes
    - name: /VirtualNetworkGateways/post/GetVirtualNetworkGatewayBGPPeerStatus
    - name: /VirtualNetworkGateways/post/ResetVirtualNetworkGateway
    - name: /VirtualNetworkGateways/patch/UpdateVirtualNetworkGatewayTags
      disabled: true
      comment: "FAILURE: Unable to find status link for polling."
    - name: /VirtualNetworkGateways/delete/DeleteVirtualNetworkGateway
    - split: p2svpngateways
    - name: /P2sVpnGateways/put/P2SVpnGatewayPut
    - name: /P2sVpnGateways/get/P2SVpnGatewayGet
    - name: /P2sVpnGateways/get/P2SVpnGatewayListByResourceGroup
    - name: /P2sVpnGateways/get/P2SVpnGatewayListBySubscription
    - name: /P2sVpnGateways/post/Disconnect VpnConnections from P2sVpn Gateway
    - name: /P2sVpnGateways/post/P2SVpnGatewayGetConnectionHealthDetailed
    - name: /P2sVpnGateways/post/P2SVpnGatewayGetConnectionHealth
    - name: /P2sVpnGateways/post/GenerateP2SVpnGatewayVPNProfile
    - name: /P2sVpnGateways/patch/P2SVpnGatewayUpdate
    - name: /P2sVpnGateways/delete/P2SVpnGatewayDelete
    - split: privatelinkservices
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /LoadBalancers/put/Create load balancer with Frontend IP in Zone 1
    - name: /PrivateLinkServices/put/Create private link service
    - name: /PrivateLinkServices/put/approve or reject private end point connection for a private link service
    - name: /PrivateLinkServices/get/Get private end point connection
    - name: /PrivateLinkServices/get/List private link service in resource group
    - name: /PrivateLinkServices/get/Get list of private link service id that can be linked to a private end point with auto approved
    - name: /PrivateLinkServices/get/Get private link service
    - name: /PrivateLinkServices/get/Get list of private link service id that can be linked to a private end point with auto approved
    - name: /PrivateLinkServices/get/List private link service in resource group
    - name: /PrivateLinkServices/get/List all private list service
    - name: /PrivateLinkServices/post/Check private link service visibility
    - name: /PrivateLinkServices/post/Check private link service visibility
    - name: /PrivateLinkServices/delete/delete private end point connection for a private link service
    - name: /PrivateLinkServices/delete/Delete private link service
    - split: expressroutecircuits
    - name: /ExpressRouteCircuits/put/Create ExpressRouteCircuit
    - name: /ExpressRouteCircuitPeerings/put/Create ExpressRouteCircuit Peerings
    - name: /ExpressRouteCircuits/put/Create ExpressRouteCircuit on ExpressRoutePort
      disabled: true
      comment: Disabled as express route port can't be created
    - name: /ExpressRouteCircuits/get/Get ExpressRoute Circuit Peering Traffic Stats
    - name: /ExpressRouteCircuits/get/Get ExpressRoute Circuit Traffic Stats
    - name: /ExpressRouteCircuits/get/Get ExpressRouteCircuit
    - name: /ExpressRouteCircuits/get/List ExpressRouteCircuits in a resource group
    - name: /ExpressRouteCircuits/get/List ExpressRouteCircuits in a subscription
    - name: /ExpressRouteCircuits/post/List Route Table Summary
      disabled: true
      comment: Disabled - not sure what device path should be
    - name: /ExpressRouteCircuits/post/List Route Tables
      disabled: true
      comment: Disabled - not sure what device path should be
    - name: /ExpressRouteCircuits/post/List ARP Table
      disabled: true
      comment: Disabled - not sure what device path should be
    - name: /ExpressRouteCircuits/patch/Update Express Route Circuit Tags
    - name: /ExpressRouteCircuits/delete/Delete ExpressRouteCircuit
      disabled: true
      comment: "Azure Error: AnotherOperationInProgress"
    - split: expressrouteports
    - name: /ExpressRoutePorts/put/ExpressRoutePortCreate
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/put/ExpressRoutePortUpdateLink
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/get/ExpressRoutePortGet
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/get/ExpressRoutePortListByResourceGroup
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/get/ExpressRoutePortList
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/patch/ExpressRoutePortUpdateTags
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - name: /ExpressRoutePorts/delete/ExpressRoutePortDelete
      disabled: true
      comment: The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'
    - split: networkwatchers
    - name: /NetworkWatchers/put/Create network watcher
    - name: /NetworkWatchers/get/Get network watcher
    - name: /NetworkWatchers/get/List network watchers
    - name: /NetworkWatchers/get/List all network watchers
    - name: /NetworkWatchers/post/Network configuration diagnostic
    - name: /NetworkWatchers/post/Get troubleshoot result
    - name: /NetworkWatchers/post/Get Azure Reachability Report
    - name: /NetworkWatchers/post/Get Available Providers List
    - name: /NetworkWatchers/post/Get flow log status
    - name: /NetworkWatchers/post/Get security group view
    - name: /NetworkWatchers/post/Check connectivity
    - name: /NetworkWatchers/post/Configure flow log
    - name: /NetworkWatchers/post/Ip flow verify
    - name: /NetworkWatchers/post/Get troubleshooting
    - name: /NetworkWatchers/post/Get Topology
    - name: /NetworkWatchers/post/Get next hop
    - name: /NetworkWatchers/patch/Update network watcher tags
    - name: /NetworkWatchers/delete/Delete network watcher
    - split: privateendpoints
    - name: /PrivateEndpoints/put/Create private endpoint with manual approval connection
    - name: /PrivateEndpoints/put/Create private endpoint
    - name: /PrivateEndpoints/get/Get private endpoint
    - name: /PrivateEndpoints/get/Get private endpoint with manual approval connection
    - name: /PrivateEndpoints/get/List private endpoints in resource group
    - name: /PrivateEndpoints/get/List all private endpoints
    - name: /PrivateEndpoints/delete/Delete private endpoint
    - split: applicationgateways
    - name: /ApplicationGateways/put/Create Application Gateway
    - name: /ApplicationGateways/get/Get Available Ssl Predefined Policy by name
    - name: /ApplicationGateways/get/Get Available Ssl Predefined Policies
    - name: /ApplicationGateways/get/Get Available Ssl Options
    - name: /ApplicationGateways/get/Get ApplicationGateway
    - name: /ApplicationGateways/get/Lists all application gateways in a resource group
    - name: /ApplicationGateways/get/Get Available Server Variables
    - name: /ApplicationGateways/get/Get Available Response Headers
    - name: /ApplicationGateways/get/Get Available Request Headers
    - name: /ApplicationGateways/get/Get Available Waf Rule Sets
    - name: /ApplicationGateways/get/Lists all application gateways in a subscription
    - name: /ApplicationGateways/post/Test Backend Health
    - name: /ApplicationGateways/post/Get Backend Health
    - name: /ApplicationGateways/post/Start Application Gateway
    - name: /ApplicationGateways/post/Stop Application Gateway
    - name: /ApplicationGateways/patch/Update Application Gateway tags
    - name: /ApplicationGateways/delete/Delete ApplicationGateway
    - split: networkprofiles
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /NetworkProfiles/put/Create network profile defaults
    - name: /NetworkProfiles/get/Get network profile with container network interfaces
    - name: /NetworkProfiles/get/Get network profile
    - name: /NetworkProfiles/get/List resource group network profiles
    - name: /NetworkProfiles/get/List all network profiles
    - name: /NetworkProfiles/patch/Update network profile tags
    - name: /NetworkProfiles/delete/Delete network profile
    - split: localnetworkgateways
    - name: /LocalNetworkGateways/put/CreateLocalNetworkGateway
    - name: /LocalNetworkGateways/get/GetLocalNetworkGateway
    - name: /LocalNetworkGateways/get/ListLocalNetworkGateways
    - name: /LocalNetworkGateways/patch/UpdateLocalNetworkGatewayTags
    - name: /LocalNetworkGateways/delete/DeleteLocalNetworkGateway
    - split: serviceendpointpolicies
    - name: /ServiceEndpointPolicies/put/Create service endpoint policy with definition
    - name: /ServiceEndpointPolicies/put/Create service endpoint policy
    - name: /ServiceEndpointPolicies/get/Get service endPoint Policy
    - name: /ServiceEndpointPolicies/get/List resource group service endpoint policies
    - name: /ServiceEndpointPolicies/get/List all service endpoint policy
    - name: /ServiceEndpointPolicies/patch/Update service endpoint policy tags
    - name: /ServiceEndpointPolicies/delete/Delete service endpoint policy
    - split: serviceendpointpolicydefinitions
    - name: /ServiceEndpointPolicies/put/Create service endpoint policy
    - name: /ServiceEndpointPolicyDefinitions/put/Create service endpoint policy definition
    - name: /ServiceEndpointPolicyDefinitions/get/Get service endpoint definition in service endpoint policy
    - name: /ServiceEndpointPolicyDefinitions/get/List service endpoint definitions in service end point policy
    - name: /ServiceEndpointPolicyDefinitions/delete/Delete service endpoint policy definitions from service endpoint policy
    - split: ddoscustompolicies
    - name: /DdosCustomPolicies/put/Create DDoS custom policy
      disabled: true
      comment: No region enabled
    - name: /DdosCustomPolicies/get/Get DDoS custom policy
      disabled: true
      comment: No region enabled
    - name: /DdosCustomPolicies/patch/DDoS Custom policy Update tags
      disabled: true
      comment: No region enabled
    - name: /DdosCustomPolicies/delete/Delete DDoS custom policy
      disabled: true
      comment: No region enabled
    - split: ddosprotectionplans
    - name: /DdosProtectionPlans/put/Create DDoS protection plan
    - name: /DdosProtectionPlans/get/Get DDoS protection plan
    - name: /DdosProtectionPlans/get/List DDoS protection plans in resource group
    - name: /DdosProtectionPlans/get/List all DDoS protection plans
    - name: /DdosProtectionPlans/patch/DDoS protection plan Update tags
    - name: /DdosProtectionPlans/delete/Delete DDoS protection plan
    - split: expressroutegateways
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /ExpressRouteGateways/put/ExpressRouteGatewayCreate
    - name: /ExpressRouteGateways/get/ExpressRouteGatewayListByResourceGroup
    - name: /ExpressRouteGateways/get/ExpressRouteGatewayListBySubscription
    - name: /ExpressRouteGateways/get/ExpressRouteGatewayGet
    - name: /ExpressRouteGateways/delete/ExpressRouteGatewayDelete
    - split: expressroutecrossconnections
    - name: /ExpressRouteCrossConnections/put/UpdateExpressRouteCrossConnection
    - name: /ExpressRouteCrossConnections/get/GetExpressRouteCrossConnection
    - name: /ExpressRouteCrossConnections/get/ExpressRouteCrossConnectionListByResourceGroup
    - name: /ExpressRouteCrossConnections/get/ExpressRouteCrossConnectionList
    - name: /ExpressRouteCrossConnections/post/GetExpressRouteCrossConnectionsRouteTableSummary
    - name: /ExpressRouteCrossConnections/post/GetExpressRouteCrossConnectionsRouteTable
    - name: /ExpressRouteCrossConnections/post/GetExpressRouteCrossConnectionsArpTable
    - name: /ExpressRouteCrossConnections/patch/UpdateExpressRouteCrossConnectionTags
    - split: virtualnetworkgatewayconnections
    - name: /VirtualNetworkGatewayConnections/put/CreateVirtualNetworkGatewayConnection_S2S
    - name: /VirtualNetworkGatewayConnections/put/SetVirtualNetworkGatewayConnectionSharedKey
    - name: /VirtualNetworkGatewayConnections/get/GetVirtualNetworkGatewayConnectionSharedKey
    - name: /VirtualNetworkGatewayConnections/get/GetVirtualNetworkGatewayConnection
    - name: /VirtualNetworkGatewayConnections/get/ListVirtualNetworkGatewayConnectionsinResourceGroup
    - name: /VirtualNetworkGatewayConnections/post/ResetVirtualNetworkGatewayConnectionSharedKey
    - name: /VirtualNetworkGatewayConnections/post/Start packet capture on virtual network gateway connection with filter
    - name: /VirtualNetworkGatewayConnections/post/Start packet capture on virtual network gateway connection without filter
    - name: /VirtualNetworkGatewayConnections/post/Stop packet capture on virtual network gateway connection
    - name: /VirtualNetworkGatewayConnections/patch/UpdateVirtualNetworkGatewayConnectionTags
    - name: /VirtualNetworkGatewayConnections/delete/DeleteVirtualNetworkGatewayConnection
    - split: vpnserverconfigurations
    - name: /VpnServerConfigurations/put/VpnServerConfigurationCreate
    - name: /VpnServerConfigurations/get/VpnServerConfigurationGet
    - name: /VpnServerConfigurations/get/VpnServerConfigurationListByResourceGroup
    - name: /VpnServerConfigurations/get/VpnServerConfigurationList
    - name: /VpnServerConfigurations/patch/VpnServerConfigurationUpdate
    - name: /VpnServerConfigurations/delete/VpnServerConfigurationDelete
    - split: networkvirtualappliances
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /NetworkVirtualAppliances/put/Create NetworkVirtualAppliance
      comment: "The resource type could not be found in the namespace 'Microsoft.Network' for api version '2020-04-01'"
    - name: /NetworkVirtualAppliances/get/Get NetworkVirtualAppliance
    - name: /NetworkVirtualAppliances/get/List all Network Virtual Appliance for a given resource group
    - name: /NetworkVirtualAppliances/get/List all Network Virtual Appliances for a given subscription
    - name: /NetworkVirtualAppliances/patch/Update NetworkVirtualAppliance
    - name: /NetworkVirtualAppliances/delete/Delete NetworkVirtualAppliance
    - split: securitypartnerproviders
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /SecurityPartnerProviders/put/Create Security Partner Provider
    - name: /SecurityPartnerProviders/get/Get Security Partner Provider
    - name: /SecurityPartnerProviders/get/List all Security Partner Providers for a given resource group
    - name: /SecurityPartnerProviders/get/List all Security Partner Providers for a given subscription
    - name: /SecurityPartnerProviders/patch/Update Security Partner Provider Tags
    - name: /SecurityPartnerProviders/delete/Delete Security Partner Provider
    - split: applicationsecuritygroups
    - name: /ApplicationSecurityGroups/put/Create application security group
    - name: /ApplicationSecurityGroups/get/Get application security group
    - name: /ApplicationSecurityGroups/get/List load balancers in resource group
    - name: /ApplicationSecurityGroups/get/List all application security groups
    - name: /ApplicationSecurityGroups/patch/Update application security group tags
    - name: /ApplicationSecurityGroups/delete/Delete application security group
    - split: webapplicationfirewallpolicies
    - name: /WebApplicationFirewallPolicies/put/Creates or updates a WAF policy within a resource group
    - name: /WebApplicationFirewallPolicies/get/Gets a WAF policy within a resource group
    - name: /WebApplicationFirewallPolicies/get/Lists all WAF policies in a resource group
    - name: /WebApplicationFirewallPolicies/get/Lists all WAF policies in a subscription
    - name: /WebApplicationFirewallPolicies/delete/Deletes a WAF policy within a resource group
    - split: vpnconnections
    - name: /VpnConnections/put/VpnConnectionPut
    - name: /VpnConnections/get/VpnConnectionGet
    - name: /VpnConnections/get/VpnConnectionList
    - name: /VpnConnections/delete/VpnConnectionDelete
    - split: loadbalancerbackendaddresspools
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /LoadBalancers/put/Create load balancer with Frontend IP in Zone 1
    - name: /LoadBalancerBackendAddressPools/put/Update load balancer backend pool with backend addresses containing virtual network and IP address defined in network interfaces.
    - name: /LoadBalancerBackendAddressPools/put/Update load balancer backend pool with backend addresses containing virtual network and  IP address.
    - name: /LoadBalancerBackendAddressPools/get/LoadBalancerBackendAddressPoolGet
    - name: /LoadBalancerBackendAddressPools/get/LoadBalancer with BackendAddressPool with BackendAddresses
    - name: /LoadBalancerBackendAddressPools/get/Load balancer with BackendAddressPool containing BackendAddresses
    - name: /LoadBalancerBackendAddressPools/get/LoadBalancerBackendAddressPoolList
    - name: /LoadBalancerBackendAddressPools/delete/BackendAddressPoolDelete
    - split: expressroutecircuitpeerings
    - name: /ExpressRouteCircuits/put/Create ExpressRouteCircuit
    - name: /ExpressRouteCircuitPeerings/put/Create ExpressRouteCircuit Peerings
    - name: /ExpressRouteCircuitPeerings/get/Get ExpressRouteCircuit Peering
    - name: /ExpressRouteCircuitPeerings/get/List ExpressRouteCircuit Peerings
    - name: /ExpressRouteCircuitPeerings/delete/Delete ExpressRouteCircuit Peerings
    - split: virtualrouterpeerings
    - name: /PublicIPAddresses/put/Create public IP address defaults
    - name: /VirtualNetworks/put/Create virtual network
    - name: /Subnets/put/Create subnet
    - name: /VirtualNetworkGateways/put/UpdateVirtualNetworkGateway
    - name: /VirtualRouters/put/Create VirtualRouter
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouterPeerings/put/Create Virtual Router Peering
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouterPeerings/get/Get Virtual Router Peering
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouterPeerings/get/List all Virtual Router Peerings for a given Virtual Router
      disabled: true
      comment: This feature is not enabled
    - name: /VirtualRouterPeerings/delete/Delete VirtualRouterPeering
      disabled: true
      comment: This feature is not enabled
    - split: connectionmonitors
    - name: /ConnectionMonitors/put/Create connection monitor V2
    - name: /ConnectionMonitors/put/Create connection monitor V1
    - name: /ConnectionMonitors/get/Get connection monitor
    - name: /ConnectionMonitors/get/List connection monitors
    - name: /ConnectionMonitors/post/Start connection monitor
    - name: /ConnectionMonitors/post/Query connection monitor
    - name: /ConnectionMonitors/post/Stop connection monitor
    - name: /ConnectionMonitors/patch/Update connection monitor tags
    - name: /ConnectionMonitors/delete/Delete connection monitor
    - split: packetcaptures
    - name: /PacketCaptures/put/Create packet capture
    - name: /PacketCaptures/get/Get packet capture
    - name: /PacketCaptures/get/List packet captures
    - name: /PacketCaptures/post/Query packet capture status
    - name: /PacketCaptures/post/Stop packet capture
    - name: /PacketCaptures/delete/Delete packet capture
    - split: flowlogs
    - name: /NetworkSecurityGroups/put/Create network security group
    - name: /FlowLogs/put/Create or update flow log
    - name: /FlowLogs/get/Get flow log
    - name: /FlowLogs/get/List connection monitors
    - name: /FlowLogs/delete/Delete flow log
    - split: hubroutetables
    - name: /HubRouteTables/put/RouteTablePut
    - name: /HubRouteTables/get/RouteTableGet
    - name: /HubRouteTables/get/RouteTableList
    - name: /HubRouteTables/delete/RouteTableDelete
    - split: expressroutecircuitauthorizations
    - name: /ExpressRouteCircuits/put/Create ExpressRouteCircuit
    - name: /ExpressRouteCircuitAuthorizations/put/Create ExpressRouteCircuit Authorization
    - name: /ExpressRouteCircuitAuthorizations/get/Get ExpressRouteCircuit Authorization
    - name: /ExpressRouteCircuitAuthorizations/get/List ExpressRouteCircuit Authorization
    - name: /ExpressRouteCircuitAuthorizations/delete/Delete ExpressRouteCircuit Authorization
    - split: expressroutecrossconnectionpeerings
    - name: /ExpressRouteCrossConnectionPeerings/put/ExpressRouteCrossConnectionBgpPeeringCreate
    - name: /ExpressRouteCrossConnectionPeerings/get/GetExpressRouteCrossConnectionBgpPeering
    - name: /ExpressRouteCrossConnectionPeerings/get/ExpressRouteCrossConnectionBgpPeeringList
    - name: /ExpressRouteCrossConnectionPeerings/delete/DeleteExpressRouteCrossConnectionBgpPeering
    - split: privatednszonegroups
    - name: /PrivateDnsZoneGroups/put/Create private dns zone group
    - name: /PrivateDnsZoneGroups/get/Get private dns zone group
    - name: /PrivateDnsZoneGroups/get/List private endpoints in resource group
    - name: /PrivateDnsZoneGroups/delete/Delete private dns zone group
    - split: expressrouteconnections
    - name: /ExpressRouteCircuits/put/Create ExpressRouteCircuit
    - name: /ExpressRouteCircuitPeerings/put/Create ExpressRouteCircuit Peerings
    - name: /VirtualWans/put/VirtualWANCreate
    - name: /VirtualHubs/put/VirtualHubPut
    - name: /ExpressRouteGateways/put/ExpressRouteGatewayCreate
    - name: /ExpressRouteConnections/put/ExpressRouteConnectionCreate
    - name: /ExpressRouteConnections/get/ExpressRouteConnectionGet
    - name: /ExpressRouteConnections/get/ExpressRouteConnectionList
    - name: /ExpressRouteConnections/delete/ExpressRouteConnectionDelete
    - split: virtualnetworkpeerings
    - name: /VirtualNetworks/put/Create virtual network
    - name: /VirtualNetworkPeerings/put/Create peering
    - name: /VirtualNetworkPeerings/get/Get peering
    - name: /VirtualNetworkPeerings/get/List peerings
    - name: /VirtualNetworkPeerings/delete/Delete peering
    - split: expressroutecircuitconnections
    - name: /ExpressRouteCircuitConnections/put/ExpressRouteCircuitConnectionCreate
    - name: /ExpressRouteCircuitConnections/get/ExpressRouteCircuitConnectionGet
    - name: /ExpressRouteCircuitConnections/get/List ExpressRouteCircuit Connection
    - name: /ExpressRouteCircuitConnections/delete/Delete ExpressRouteCircuit

    - split: other
    - name: /VpnSiteLinkConnections/get/VpnSiteLinkConnectionGet
    - name: /DefaultSecurityRules/get/DefaultSecurityRuleGet
    - name: /PeerExpressRouteCircuitConnections/get/PeerExpressRouteCircuitConnectionGet
    - name: /LoadBalancerFrontendIPConfigurations/get/LoadBalancerFrontendIPConfigurationGet
    - name: /ResourceNavigationLinks/get/Get Resource Navigation Links
    - name: /ServiceAssociationLinks/get/Get Service Association Links
    - name: /NetworkInterfaceIPConfigurations/get/NetworkInterfaceIPConfigurationGet
    - name: /LoadBalancerLoadBalancingRules/get/LoadBalancerLoadBalancingRuleGet
    - name: /VpnLinkConnections/get/VpnSiteLinkConnectionList
    - name: /HubVirtualNetworkConnections/get/HubVirtualNetworkConnectionGet
    - name: /PeerExpressRouteCircuitConnections/get/List Peer ExpressRouteCircuit Connection
    - name: /LoadBalancerOutboundRules/get/LoadBalancerOutboundRuleGet
    - name: /DefaultSecurityRules/get/DefaultSecurityRuleList
    - name: /ExpressRouteLinks/get/ExpressRouteLinkGet
    - name: /VpnSiteLinks/get/VpnSiteGet
    - name: /LoadBalancerFrontendIPConfigurations/get/LoadBalancerFrontendIPConfigurationList
    - name: /HubVirtualNetworkConnections/get/HubVirtualNetworkConnectionList
    - name: /NetworkInterfaceIPConfigurations/get/NetworkInterfaceIPConfigurationList
    - name: /LoadBalancerProbes/get/LoadBalancerProbeGet
    - name: /AvailablePrivateEndpointTypes/get/Get available PrivateEndpoint types in the resource group
    - name: //get/supportedSecurityProviders
    - name: /NetworkInterfaceLoadBalancers/get/NetworkInterfaceLoadBalancerList
    - name: /LoadBalancerLoadBalancingRules/get/LoadBalancerLoadBalancingRuleList
    - name: /LoadBalancerNetworkInterfaces/get/LoadBalancerNetworkInterfaceListVmss
    - name: /LoadBalancerNetworkInterfaces/get/LoadBalancerNetworkInterfaceListSimple
    - name: /AvailableServiceAliases/get/Get available service aliases in the resource group
    - name: /ExpressRouteLinks/get/ExpressRouteLinkGet
    - name: /LoadBalancerOutboundRules/get/LoadBalancerOutboundRuleList
    - name: /AvailableResourceGroupDelegations/get/Get available delegations in the resource group
    - name: /LoadBalancerProbes/get/LoadBalancerProbeList
    - name: /VpnSiteLinks/get/VpnSiteLinkListByVpnSite
    - name: /AvailableEndpointServices/get/EndpointServicesList
    - name: /AvailablePrivateEndpointTypes/get/Get available PrivateEndpoint types
    - name: //get/Check Dns Name Availability
    - name: /AvailableServiceAliases/get/Get available service aliases
    - name: /AvailableDelegations/get/Get available delegations
    - name: /ExpressRoutePortsLocations/get/ExpressRoutePortsLocationGet
    - name: /ServiceTags/get/Get list of service tags
    - name: /Usages/get/List usages
    - name: /Usages/get/List usages spaced location
    - name: /ExpressRouteServiceProviders/get/List ExpressRoute providers
    - name: /ExpressRoutePortsLocations/get/ExpressRoutePortsLocationList
    - name: /AzureFirewallFqdnTags/get/List all Azure Firewall FQDN Tags for a given subscription
    - name: /BgpServiceCommunities/get/ServiceCommunityList
    - name: /Operations/get/Get a list of operations for a resource provider
    - name: //post/Deletes the specified active session
    - name: //post/Create Bastion Shareable Links for the request VMs
    - name: //post/Delete Bastion Shareable Links for the request VMs
    - name: /VpnServerConfigurationsAssociatedWithVirtualWan/post/GetVirtualWanVpnServerConfigurations
    - name: //post/Returns the Bastion Shareable Links for the request VMs
    - name: //post/Returns a list of currently active sessions on the Bastion
    - name: //post/GenerateVirtualWanVpnServerConfigurationVpnProfile
    - name: /VpnSitesConfiguration/post/VpnSitesConfigurationDownload
```