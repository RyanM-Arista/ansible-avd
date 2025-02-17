=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>ntp</samp>](## "ntp") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;local_interface</samp>](## "ntp.local_interface") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;name</samp>](## "ntp.local_interface.name") | String |  |  |  | Source interface |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;vrf</samp>](## "ntp.local_interface.vrf") | String |  |  |  | VRF name |
    | [<samp>&nbsp;&nbsp;servers</samp>](## "ntp.servers") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- name</samp>](## "ntp.servers.[].name") | String |  |  |  | IP or hostname e.g., 2.2.2.55, ie.pool.ntp.org |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;burst</samp>](## "ntp.servers.[].burst") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;iburst</samp>](## "ntp.servers.[].iburst") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;key</samp>](## "ntp.servers.[].key") | Integer |  |  | Min: 1<br>Max: 65535 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;local_interface</samp>](## "ntp.servers.[].local_interface") | String |  |  |  | Source interface |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;maxpoll</samp>](## "ntp.servers.[].maxpoll") | Integer |  |  | Min: 3<br>Max: 17 | Value of maxpoll between 3 - 17 (Logarithmic) |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;minpoll</samp>](## "ntp.servers.[].minpoll") | Integer |  |  | Min: 3<br>Max: 17 | Value of minpoll between 3 - 17 (Logarithmic) |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;preferred</samp>](## "ntp.servers.[].preferred") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;version</samp>](## "ntp.servers.[].version") | Integer |  |  | Min: 1<br>Max: 4 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vrf</samp>](## "ntp.servers.[].vrf") | String |  |  |  | VRF name |
    | [<samp>&nbsp;&nbsp;authenticate</samp>](## "ntp.authenticate") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;authenticate_servers_only</samp>](## "ntp.authenticate_servers_only") | Boolean |  |  |  |  |
    | [<samp>&nbsp;&nbsp;authentication_keys</samp>](## "ntp.authentication_keys") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- id</samp>](## "ntp.authentication_keys.[].id") | Integer | Required, Unique |  | Min: 1<br>Max: 65534 | Key identifier |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hash_algorithm</samp>](## "ntp.authentication_keys.[].hash_algorithm") | String |  |  | Valid Values:<br>- md5<br>- sha1 |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;key</samp>](## "ntp.authentication_keys.[].key") | String |  |  |  | Obfuscated key |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;key_type</samp>](## "ntp.authentication_keys.[].key_type") | String |  |  | Valid Values:<br>- 0<br>- 7<br>- 8a |  |
    | [<samp>&nbsp;&nbsp;trusted_keys</samp>](## "ntp.trusted_keys") | String |  |  |  | List of trusted-keys as string ex. 10-12,15 |

=== "YAML"

    ```yaml
    ntp:
      local_interface:
        name: <str>
        vrf: <str>
      servers:
        - name: <str>
          burst: <bool>
          iburst: <bool>
          key: <int>
          local_interface: <str>
          maxpoll: <int>
          minpoll: <int>
          preferred: <bool>
          version: <int>
          vrf: <str>
      authenticate: <bool>
      authenticate_servers_only: <bool>
      authentication_keys:
        - id: <int>
          hash_algorithm: <str>
          key: <str>
          key_type: <str>
      trusted_keys: <str>
    ```
