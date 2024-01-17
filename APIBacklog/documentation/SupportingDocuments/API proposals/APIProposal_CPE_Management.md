| **Field** | Description |
| --- | --- |
| API family name | CPE Management |
| API family owner | Charter Communications |
| API family summary | Service enabling API for customer premises equipment (CPE) management, focusing on managing Isolated Networks and device reboot requests. It allows application developers to create, modify, or remove isolated networks and reboot network operator-supplied network access devices. |
|| An isolated network is a network access configuration where each configuration is for a logically separated Local Area Network (LAN) within the scope of a single network device. Application developers can create, modify, or remove these networks which could be useful in scenarios such as: |
|| A request to reboot a network operator-supplied network access device. Useful for recovering from faulty network states by rebooting gateway devices or rebooting multiple devices at various locations. |
| Technical viability | Involves creating, modifying, or deleting isolated networks using `/isolated-networks` endpoints, iterating over locations via `/service-sites` endpoints, and rebooting devices through `/reboot-requests` endpoints. Additional scope available for reconciling information about service sites and configuring devices. |
| Commercial viability | Aimed at value-added resellers and short-term rental agencies, suitable for managing home routers and networks. Provides functionalities like managing isolated networks and rebooting devices. |
| YAML code available? | YES <br> |
| Validated in lab/productive environments? | YES <br> |
| Validated with real customers? | NO (Planned pilot 2024) <br> |
| Validated with operators? | Liberty Global, Vodafone, VodafoneZiggo, Charter, CableLabs (completed PoC) </em> |
| Supporters in API Backlog Working Group | Liberty Global, Vodafone, VodafoneZiggo, Charter, CableLabs |