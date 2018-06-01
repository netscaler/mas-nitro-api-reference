#ns_servicegroup

Configuration for NS Service Group Information resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>hostname</td><td>&lt;String></td><td>Read-write</td><td>Hostname of the managed device.<br>Minimum length = 1<br>Maximum length = 256</td></tr><tr><td>svc_grp_mem_port</td><td>&lt;Integer></td><td>Read-write</td><td>Service Group Member Port.<br>Minimum value = 1<br>Maximum value =</td></tr><tr><td>svc_grp_name</td><td>&lt;String></td><td>Read-write</td><td>Service Group Name.<br>Minimum length = 1<br>Maximum length = 100</td></tr><tr><td>ns_ip_address</td><td>&lt;String></td><td>Read-write</td><td>NS IP Address.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>svc_grp_mem_ip_address</td><td>&lt;String></td><td>Read-write</td><td>Service Group Member IP Address.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key.</td></tr><tr><td>save_config</td><td>&lt;Boolean></td><td>Read-write</td><td>Save configuration after enable/disable.</td></tr><tr><td>lb_id</td><td>&lt;String></td><td>Read-write</td><td>LB ID.</td></tr><tr><td>vsvr_name</td><td>&lt;String></td><td>Read-write</td><td>Vserver Name.<br>Minimum length = 1<br>Maximum length = 100</td></tr><tr><td>svr_name</td><td>&lt;String></td><td>Read-write</td><td>Server Member Name.<br>Minimum length = 1<br>Maximum length = 100</td></tr><tr><td>delay</td><td>&lt;Double></td><td>Read-write</td><td>Time, in seconds, allocated to the NetScaler appliance for a graceful shutdown of the service.</td></tr><tr><td>svr_id</td><td>&lt;String></td><td>Read-write</td><td>Server ID.</td></tr><tr><td>graceful</td><td>&lt;Boolean></td><td>Read-write</td><td>Graceful shutdown of Service..</td></tr><tr><td>svrstate</td><td>&lt;String></td><td>Read-only</td><td>Service State.</td></tr><tr><td>svc_grp_state_timestamp</td><td>&lt;Double></td><td>Read-only</td><td>Service Group Last State Change Time.</td></tr><tr><td>poll_time</td><td>&lt;Integer></td><td>Read-only</td><td>Last Polling Time.</td></tr><tr><td>display_name</td><td>&lt;String></td><td>Read-only</td><td>Display Name.</td></tr><tr><td>svc_grp_effective_state</td><td>&lt;String></td><td>Read-only</td><td>Service Group Effective State.</td></tr><tr><td>partition_name</td><td>&lt;String></td><td>Read-only</td><td>Partition Name.</td></tr><tr><td>comment</td><td>&lt;String></td><td>Read-only</td><td>Comment.</td></tr><tr><td>svc_grp_mem_state</td><td>&lt;String></td><td>Read-only</td><td>Service Group Member State.</td></tr><tr><td>svc_grp_mem_type</td><td>&lt;String></td><td>Read-only</td><td>Service Group Member Type.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[ENABLE](#e)| [POLL]()| [GET]()| [DISABLE](#di)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###enable



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_servicegroup?action=enable;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###poll



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_servicegroup?action=poll;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_servicegroup
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###disable



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_servicegroup?action=disable;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>


