#metering_export

Configuration for Metering Data Export resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>file_name</td><td>&lt;String></td><td>Read-write</td><td>File Name.<br>Minimum length = 1<br>Maximum length = 512</td></tr><tr><td>ip_address</td><td>&lt;String></td><td>Read-write</td><td>IP Address for this VM device for which metering data export is required.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>end_time</td><td>&lt;Double></td><td>Read-only</td><td>End Time of interval for which export is generated.</td></tr><tr><td>file_size</td><td>&lt;Integer></td><td>Read-only</td><td>file_size.</td></tr><tr><td>start_time</td><td>&lt;Double></td><td>Read-only</td><td>Start Time of interval for which export is generated.</td></tr><tr><td>file_last_modified</td><td>&lt;String></td><td>Read-only</td><td>Last Modified.</td></tr><tr><td>duration</td><td>&lt;String></td><td>Read-only</td><td>Interval Duration for which export is generated.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[DELETE](#d)| [GET (ALL)](#get-)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/metering_export/file_name_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/metering_export
<b>HTTP Method:</b>null
<b>Response Payload: </b>


