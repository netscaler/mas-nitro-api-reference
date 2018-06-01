#appscore_threshold_config

Configuration for Additional Server node information resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>lowCPU</td><td>&lt;Double></td><td>Read-write</td><td>Low CPU Threshold.</td></tr><tr><td>lowThreatScore</td><td>&lt;Double></td><td>Read-write</td><td>Low Threat Score.</td></tr><tr><td>lowNicDisCards</td><td>&lt;Double></td><td>Read-write</td><td>Low NIC Discards SLA.</td></tr><tr><td>highCPU</td><td>&lt;Double></td><td>Read-write</td><td>High CPU Threshold.</td></tr><tr><td>highThreatScore</td><td>&lt;Double></td><td>Read-write</td><td>High Threat Score.</td></tr><tr><td>lowMemory</td><td>&lt;Double></td><td>Read-write</td><td>Low Memory Threshold.</td></tr><tr><td>responseTimeSLA</td><td>&lt;Double></td><td>Read-write</td><td>Response Time Threshold.</td></tr><tr><td>highNicCongestion</td><td>&lt;Double></td><td>Read-write</td><td>High NIC Congestion.</td></tr><tr><td>lowNicCongestion</td><td>&lt;Double></td><td>Read-write</td><td>Low NIC Congestion.</td></tr><tr><td>highNicDisCards</td><td>&lt;Double></td><td>Read-write</td><td>High NIC Discards SLA.</td></tr><tr><td>highSurgeQ</td><td>&lt;Double></td><td>Read-write</td><td>Higher Surge Queue Threshold.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id.</td></tr><tr><td>lowSurgeQ</td><td>&lt;Double></td><td>Read-write</td><td>Lower Surge Queue Threshold.</td></tr><tr><td>highMemory</td><td>&lt;Double></td><td>Read-write</td><td>High Memory Threshold.</td></tr><tr><td>activeServicesSLA</td><td>&lt;Double></td><td>Read-write</td><td>Active Services Threshold.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[ADD]()| [DELETE](#d)| [GET (ALL)](#get-)| [GET]()| [UPDATE](#u)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###add



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/appscore_threshold_config?onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/appscore_threshold_config/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/appscore_threshold_config
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/appscore_threshold_config/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###update



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/appscore_threshold_config/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>


