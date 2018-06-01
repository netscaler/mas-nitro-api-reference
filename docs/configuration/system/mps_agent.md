#mps_agent

Configuration for MPS Agent information resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>deployment_status</td><td>&lt;Boolean></td><td>Read-write</td><td>Deployment status of this node..</td></tr><tr><td>hostname</td><td>&lt;String></td><td>Read-write</td><td>Hostname of the agent.</td></tr><tr><td>down_count</td><td>&lt;Integer></td><td>Read-write</td><td>Shows for how long agent was down, each value of count increases after every 10 seconds.</td></tr><tr><td>state</td><td>&lt;String></td><td>Read-write</td><td>Agent state.</td></tr><tr><td>password</td><td>&lt;String></td><td>Read-write</td><td>Password.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>tenant</td><td>&lt;String></td><td>Read-write</td><td>Tenant.</td></tr><tr><td>public_key</td><td>&lt;String></td><td>Read-write</td><td>public key for agent.</td></tr><tr><td>platform</td><td>&lt;String></td><td>Read-write</td><td>Platform.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for agent registered with NMX Cloud..</td></tr><tr><td>instance_id</td><td>&lt;String></td><td>Read-write</td><td>Unique ID of device provided by Global Trust Service.</td></tr><tr><td>version</td><td>&lt;String></td><td>Read-write</td><td>version..</td></tr><tr><td>datacenter_id</td><td>&lt;String></td><td>Read-write</td><td>Datacenter Id is system generated key for data center.</td></tr><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Agent IP Address.</td></tr><tr><td>rpt_sample_time</td><td>&lt;Double></td><td>Read-write</td><td>Report Sample time..</td></tr><tr><td>discovery_time</td><td>&lt;Double></td><td>Read-write</td><td>discovery time.</td></tr><tr><td>username</td><td>&lt;String></td><td>Read-write</td><td>username configured on DB node..<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>certificate</td><td>&lt;String></td><td>Read-write</td><td>Name of ABDP Certificate File.</td></tr><tr><td>connector_ips</td><td>&lt;String></td><td>Read-write</td><td>Comma separated list of connector node IPs..</td></tr><tr><td>bulk_request_ipaddress</td><td>&lt;String></td><td>Read-write</td><td>ABDP IP Address..<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>upgrade_version</td><td>&lt;String></td><td>Read-write</td><td>Represents the next version the agent should upgrade to.</td></tr><tr><td>registered_devices</td><td>&lt;managed_device[]></td><td>Read-write</td><td>List of registered devices..</td></tr><tr><td>bulk_request_port</td><td>&lt;Integer></td><td>Read-write</td><td>Port number for ABDP.</td></tr><tr><td>city</td><td>&lt;String></td><td>Read-write</td><td>City.</td></tr><tr><td>mas_version</td><td>&lt;String></td><td>Read-write</td><td>MAS server's current version.</td></tr><tr><td>url</td><td>&lt;String></td><td>Read-write</td><td>URL of ABDP Certificate File Location.</td></tr><tr><td>country</td><td>&lt;String></td><td>Read-write</td><td>Country.</td></tr><tr><td>region</td><td>&lt;String></td><td>Read-write</td><td>Region.</td></tr><tr><td>port</td><td>&lt;Integer></td><td>Read-write</td><td>Port number for ABDP Certificate file location.</td></tr><tr><td>zipcode</td><td>&lt;String></td><td>Read-write</td><td>Zipcode of location.<br>Maximum length = 32</td></tr><tr><td>server_time</td><td>&lt;Double></td><td>Read-write</td><td>MAS server's Epoch time.</td></tr><tr><td>loc</td><td>&lt;String></td><td>Read-write</td><td>Location - latitude and longitude.</td></tr><tr><td>agent_msg_router_url</td><td>&lt;String></td><td>Read-write</td><td>URL for router.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[DELETE](#d)| [GET (ALL)](#get-)| [GET]()


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_agent/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_agent
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_agent/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>


