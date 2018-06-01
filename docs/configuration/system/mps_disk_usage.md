#mps_disk_usage

Configuration for Available Disks Usage resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>parent_name</td><td>&lt;String></td><td>Read-write</td><td>.</td></tr><tr><td>parent_id</td><td>&lt;String></td><td>Read-write</td><td>.</td></tr><tr><td>disk_partition</td><td>&lt;String></td><td>Read-write</td><td>Disk Partition.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>.</td></tr><tr><td>free_space</td><td>&lt;Double></td><td>Read-only</td><td>Free space available in KB.</td></tr><tr><td>disk_usage</td><td>&lt;Double></td><td>Read-only</td><td>Disk Usage (%).</td></tr><tr><td>used_space</td><td>&lt;Double></td><td>Read-only</td><td>Used space available in KB.</td></tr><tr><td>disk_name</td><td>&lt;String></td><td>Read-only</td><td>Disk Name.</td></tr><tr><td>total_space</td><td>&lt;Double></td><td>Read-only</td><td>Total space in KB.</td></tr><tr><td>disk_slice</td><td>&lt;String></td><td>Read-only</td><td>Disk Slice.</td></tr><tr><td>disk_capacity</td><td>&lt;Double></td><td>Read-only</td><td>Disk Total Capacity in KB.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[GET (ALL)](#get-)| [GET]()


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_disk_usage
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_disk_usage/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>


