=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>ipv6_static_routes</samp>](## "ipv6_static_routes") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;- vrf</samp>](## "ipv6_static_routes.[].vrf") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;destination_address_prefix</samp>](## "ipv6_static_routes.[].destination_address_prefix") | String |  |  |  | IPv6 Network/Mask |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;interface</samp>](## "ipv6_static_routes.[].interface") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;gateway</samp>](## "ipv6_static_routes.[].gateway") | String |  |  |  | IPv6 Address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;track_bfd</samp>](## "ipv6_static_routes.[].track_bfd") | Boolean |  |  |  | Track next-hop using BFD |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;distance</samp>](## "ipv6_static_routes.[].distance") | Integer |  |  | Min: 1<br>Max: 255 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;tag</samp>](## "ipv6_static_routes.[].tag") | Integer |  |  | Min: 0<br>Max: 4294967295 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;name</samp>](## "ipv6_static_routes.[].name") | String |  |  |  | Description |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;metric</samp>](## "ipv6_static_routes.[].metric") | Integer |  |  | Min: 0<br>Max: 4294967295 |  |

=== "YAML"

    ```yaml
    ipv6_static_routes:
      - vrf: <str>
        destination_address_prefix: <str>
        interface: <str>
        gateway: <str>
        track_bfd: <bool>
        distance: <int>
        tag: <int>
        name: <str>
        metric: <int>
    ```
