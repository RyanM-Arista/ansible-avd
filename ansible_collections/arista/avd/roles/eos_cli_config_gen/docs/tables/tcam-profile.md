=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>tcam_profile</samp>](## "tcam_profile") | Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;system</samp>](## "tcam_profile.system") | String |  |  |  | TCAM profile name to activate<br> |
    | [<samp>&nbsp;&nbsp;profiles</samp>](## "tcam_profile.profiles") | List, items: Dictionary |  |  |  |  |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;- name</samp>](## "tcam_profile.profiles.[].name") | String | Required, Unique |  |  | Tcam-Profile Name |
    | [<samp>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;config</samp>](## "tcam_profile.profiles.[].config") | String | Required |  |  | TCAM Profile Config. Since these can be very long, it is often a good idea to import the config from a file.<br>Example: "{{ lookup('file', 'TCAM_TRAFFIC_POLICY.conf') }}" |

=== "YAML"

    ```yaml
    tcam_profile:
      system: <str>
      profiles:
        - name: <str>
          config: <str>
    ```
