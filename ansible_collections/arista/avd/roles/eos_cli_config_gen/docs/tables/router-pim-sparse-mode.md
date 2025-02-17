=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>router_pim_sparse_mode</samp>](## "router_pim_sparse_mode") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;ipv4</samp>](## "router_pim_sparse_mode.ipv4") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;bfd</samp>](## "router_pim_sparse_mode.ipv4.bfd") | Boolean |  |  |  | Enable/Disable BFD |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;ssm_range</samp>](## "router_pim_sparse_mode.ipv4.ssm_range") | String |  |  |  | IPv4 Prefix associated with SSM |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;rp_addresses</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- address</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].address") | String | Required, Unique |  |  | RP Address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;groups</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].groups") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].groups.[].&lt;str&gt;") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;access_lists</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].access_lists") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].access_lists.[].&lt;str&gt;") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;priority</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].priority") | Integer |  |  | Min: 0<br>Max: 255 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hashmask</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].hashmask") | Integer |  |  | Min: 0<br>Max: 32 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;override</samp>](## "router_pim_sparse_mode.ipv4.rp_addresses.[].override") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;anycast_rps</samp>](## "router_pim_sparse_mode.ipv4.anycast_rps") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- address</samp>](## "router_pim_sparse_mode.ipv4.anycast_rps.[].address") | String | Required, Unique |  |  | Anycast RP Address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;other_anycast_rp_addresses</samp>](## "router_pim_sparse_mode.ipv4.anycast_rps.[].other_anycast_rp_addresses") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- address</samp>](## "router_pim_sparse_mode.ipv4.anycast_rps.[].other_anycast_rp_addresses.[].address") | String | Required, Unique |  |  | Other Anycast RP Address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;register_count</samp>](## "router_pim_sparse_mode.ipv4.anycast_rps.[].other_anycast_rp_addresses.[].register_count") | Integer |  |  |  |  |
    | [<samp>&nbsp;&nbsp;vrfs</samp>](## "router_pim_sparse_mode.vrfs") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- name</samp>](## "router_pim_sparse_mode.vrfs.[].name") | String | Required, Unique |  |  | VRF Name |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ipv4</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bfd</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.bfd") | Boolean |  |  |  | Enable/Disable BFD |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rp_addresses</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- address</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].address") | String | Required |  |  | RP Address |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;groups</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].groups") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].groups.[].&lt;str&gt;") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;access_lists</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].access_lists") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].access_lists.[].&lt;str&gt;") | String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;priority</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].priority") | Integer |  |  | Min: 0<br>Max: 255 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hashmask</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].hashmask") | Integer |  |  | Min: 0<br>Max: 32 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;override</samp>](## "router_pim_sparse_mode.vrfs.[].ipv4.rp_addresses.[].override") | Boolean |  |  |  |  |

=== "YAML"

    ```yaml
    router_pim_sparse_mode:
      ipv4:
        bfd: <bool>
        ssm_range: <str>
        rp_addresses:
          - address: <str>
            groups:
              - <str>
            access_lists:
              - <str>
            priority: <int>
            hashmask: <int>
            override: <bool>
        anycast_rps:
          - address: <str>
            other_anycast_rp_addresses:
              - address: <str>
                register_count: <int>
      vrfs:
        - name: <str>
          ipv4:
            bfd: <bool>
            rp_addresses:
              - address: <str>
                groups:
                  - <str>
                access_lists:
                  - <str>
                priority: <int>
                hashmask: <int>
                override: <bool>
    ```
