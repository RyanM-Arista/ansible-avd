=== "Table"

    | Variable | Type | Required | Default | Value Restrictions | Description |
    | -------- | ---- | -------- | ------- | ------------------ | ----------- |
    | [<samp>is_deployed</samp>](## "is_deployed") | Boolean |  | `True` |  | Is device already deployed in the fabric.<br>When set to false, interfaces toward this device may be shutdown depending on the `shutdown_interfaces_towards_undeployed_peers` setting.<br>Furthermore `eos_config_deploy_cvp` will not attempt to move or apply configurations to the device.<br> |

=== "YAML"

    ```yaml
    is_deployed: <bool>
    ```
