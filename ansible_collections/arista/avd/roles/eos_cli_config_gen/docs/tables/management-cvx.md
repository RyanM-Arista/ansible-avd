=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>management_cvx</samp>](## "management_cvx") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;shutdown</samp>](## "management_cvx.shutdown") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;server_hosts</samp>](## "management_cvx.server_hosts") | List, items: String |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- &lt;str&gt;</samp>](## "management_cvx.server_hosts.[].&lt;str&gt;") | String |  |  |  | IP or hostname |
    | [<samp>&nbsp;&nbsp;source_interface</samp>](## "management_cvx.source_interface") | String |  |  |  | Interface name |
    | [<samp>&nbsp;&nbsp;vrf</samp>](## "management_cvx.vrf") | String |  |  |  | VRF Name |

=== "YAML"

    ```yaml
    management_cvx:
      shutdown: <bool>
      server_hosts:
        - <str>
      source_interface: <str>
      vrf: <str>
    ```
