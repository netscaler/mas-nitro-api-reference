#ns_conf

Configuration for ns.conf file on NetScaler resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>diff_status</td><td>&lt;String></td><td>Read-write</td><td>Tells whether a diff exists between running and saved configuration on NS.</td></tr><tr><td>ns_ip_address</td><td>&lt;String></td><td>Read-write</td><td>List of NetScaler IP Address.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>last_updated_time</td><td>&lt;Integer></td><td>Read-write</td><td>Last Updated Time.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all ns.conf files.</td></tr><tr><td>templatediff_status</td><td>&lt;String></td><td>Read-write</td><td>Tells whether a diff exists between templates associated to the NS and the running configuration.</td></tr><tr><td>last_updated_times</td><td>&lt;String[]></td><td>Read-write</td><td>List of last updated times for templates.</td></tr><tr><td>diff_reportname</td><td>&lt;String></td><td>Read-only</td><td>Name of the SavedVsRunning diff reportname.</td></tr><tr><td>hostname</td><td>&lt;String></td><td>Read-only</td><td>Host Name of the device.</td></tr><tr><td>display_name</td><td>&lt;String></td><td>Read-only</td><td>Display Name of the device.</td></tr><tr><td>device_name</td><td>&lt;String></td><td>Read-only</td><td>Name of the device.</td></tr><tr><td>templatediff_reportname</td><td>&lt;String></td><td>Read-only</td><td>Name of the Template diff reports.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[INVENTORY](#inve)| [DOWNLOAD_CONF](#download)| [DELETE](#d)| [GET (ALL)](#get-)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###inventory



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_conf?action=inventory;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###download_conf



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_conf?action=download_conf;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_conf?action=delete;onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ns_conf
<b>HTTP Method:</b>null
<b>Response Payload: </b>


