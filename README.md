# NetworkSecurityProject
Year 1 Sem 2

# Low-Cost Flow-Based Security Solutions for Smart-Home IoT Devices

The rapid proliferation of Internet of Things (IoT) devices
is giving rise to “smart-homes” that can be monitored and
controlled remotely over the Internet. Consumers can now
control their lighting systems from anywhere [1], receive alerts
on their mobile phone when smoke is detected in the house
[2], monitor their kids from afar [3], and turn appliances
on/off while driving to/from work [4]. Recent surveys in the
US have shown that many consumers are willing to pay
in excess of $500 for a fully-equipped smart-home, citing
personal or family safety, property protection, lighting/energy
management, and pet monitoring as top motivators [5].
The increasing prevalence of smart-homes with Internet-
connected devices creates security concerns at unprecedented
levels. An eavesdropper can illegitimately snoop into family
activities, and a malicious entity can take control of the home
to either harm the household or to use it as a launch-pad for
attacks into other domains. The vulnerabilities of existing IoT
devices have been documented by several earlier studies [6],
[7], and there is evidence of anecdotal [8] as well as large-
scale attacks [9] on IoT devices.
Securing IoT devices from attacks remains a formidable
challenge. The large heterogeneity in IoT devices, each with
its own hardware, firmware, and software, makes the security
vulnerabilities diverse and the attack vectors manifold. Worse,
device manufacturers have been lax in embedding security in
Funding for this project was provided by the Australian Research Council
(ARC) Linkage Grant LP150100666.
consumer IoT devices, dissuaded by low margins, time-to-
market pressures, and limited resources. One could argue that
the home router, by virtue of its NAT/firewall functionality,
provides an effective protection against external attacks by
dropping unsolicited Internet traffic directed to household IoT
devices. However, our recent work in [10] has shown that even
this perimeter defense can be bypassed via malware embedded
into mobile Apps; such malware can scout the internal network
for vulnerable IoT devices, and disable the home firewall to
allow Internet attacks on such devices.
We believe that a promising approach to the above problem
is to embed security solutions at the network-level, whereby
network traffic to/from IoT devices is monitored to detect
(and block) attacks, much the way today’s intrusion detection
systems (IDS) monitor enterprise network traffic for security
threats. Indeed, our prior work [11] has demonstrated the
utility of traffic-flow monitoring in securing access to devices
such as light-bulbs in the smart-home; concurrently, work
in [12] has developed a method for specifying IoT security
policies, that are then applied to the network data-plane traffic
via specialized middle-boxes (termed µmboxes).
While the above methods show promise in securing smart-
homes at the network-level, it remains unclear what their
cost/benefit trade-offs are, particularly since inspection of net-
work traffic can involve significant costs that may be difficult
to recover in a residential market wherein profit margins are
low. In this paper, we undertake an evaluation of the cost-
benefit trade-offs of a flow-level approach (that predominantly
uses information about active flows in the network) against a
packet-level approach (that looks into the content of the data
packets) for securing smart-home IoT devices. In this context,
our contributions are:

- Mitigating DoS attack inside Home Networks
- Detecting and Prevetning SlowHttp Soloris Attacks
- Creating custom firewall to prevent external attacks
- Analysing traffic on SSDP & UPnP ports to detect and block traffic
