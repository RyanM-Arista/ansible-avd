=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>address_locking</samp>](## "address_locking") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;dhcp_servers_ipv4</samp>](## "address_locking.dhcp_servers_ipv4") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "address_locking.dhcp_servers_ipv4.[].&lt;str&gt;") | String |  |  |  | DHCP server IPv4 address |
    | [<samp>&nbsp;&nbsp;disabled</samp>](## "address_locking.disabled") | Boolean |  |  |  | Disable IP locking on configured ports |
    | [<samp>&nbsp;&nbsp;leases</samp>](## "address_locking.leases") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- ip</samp>](## "address_locking.leases.[].ip") | String | Required |  |  | IP address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mac</samp>](## "address_locking.leases.[].mac") | String | Required |  |  | MAC address (hhhh.hhhh.hhhh or hh:hh:hh:hh:hh:hh) |
    | [<samp>&nbsp;&nbsp;local_interface</samp>](## "address_locking.local_interface") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;locked_address</samp>](## "address_locking.locked_address") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;expiration_mac_disabled</samp>](## "address_locking.locked_address.expiration_mac_disabled") | Boolean |  |  |  | Configure deauthorizing locked addresses upon MAC aging out |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;ipv4_enforcement_disabled</samp>](## "address_locking.locked_address.ipv4_enforcement_disabled") | Boolean |  |  |  | Configure enforcement for locked IPv4 addresses |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;ipv6_enforcement_disabled</samp>](## "address_locking.locked_address.ipv6_enforcement_disabled") | Boolean |  |  |  | Configure enforcement for locked IPv6 addresses |

=== "YAML"

    ```yaml
    address_locking:
      dhcp_servers_ipv4:
        - <str>
      disabled: <bool>
      leases:
        - ip: <str>
          mac: <str>
      local_interface: <str>
      locked_address:
        expiration_mac_disabled: <bool>
        ipv4_enforcement_disabled: <bool>
        ipv6_enforcement_disabled: <bool>
    ```
