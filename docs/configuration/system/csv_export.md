#csv_export

Configuration for CSV Export resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>report_end_time</td><td>&lt;Double></td><td>Read-write</td><td>Report end time..</td></tr><tr><td>order_by</td><td>&lt;String></td><td>Read-write</td><td>Order By.<br>Maximum length = 32</td></tr><tr><td>args</td><td>&lt;String></td><td>Read-write</td><td>args.</td></tr><tr><td>report_start_time</td><td>&lt;Double></td><td>Read-write</td><td>Report start time..</td></tr><tr><td>resource_id</td><td>&lt;String></td><td>Read-write</td><td>Resource id.<br>Maximum length = 512</td></tr><tr><td>asc</td><td>&lt;String></td><td>Read-write</td><td>asc.<br>Maximum length = 32</td></tr><tr><td>duration_summary</td><td>&lt;String></td><td>Read-write</td><td>Duration summary..<br>Maximum length = 16</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is CSV export Id.<br>Maximum length = 32</td></tr><tr><td>section_title</td><td>&lt;String></td><td>Read-write</td><td>Section title.<br>Maximum length = 512</td></tr><tr><td>attrs</td><td>&lt;String></td><td>Read-write</td><td>attrs.</td></tr><tr><td>is_count</td><td>&lt;String></td><td>Read-write</td><td>is_count.<br>Maximum length = 32</td></tr><tr><td>filter</td><td>&lt;String></td><td>Read-write</td><td>filter.</td></tr><tr><td>detailview</td><td>&lt;String></td><td>Read-write</td><td>detailview.<br>Maximum length = 64</td></tr><tr><td>duration</td><td>&lt;String></td><td>Read-write</td><td>Duration.<br>Maximum length = 64</td></tr><tr><td>cr_enabled</td><td>&lt;String></td><td>Read-write</td><td>CR Enabled..<br>Maximum length = 16</td></tr><tr><td>sla_enabled</td><td>&lt;String></td><td>Read-write</td><td>SLA Enabled..<br>Maximum length = 16</td></tr><tr><td>type</td><td>&lt;String></td><td>Read-write</td><td>Type.<br>Maximum length = 32</td></tr><tr><td>resource_name</td><td>&lt;String></td><td>Read-write</td><td>Resource name.<br>Minimum length = 1<br>Maximum length = 255</td></tr><tr><td>csv_mapping_id</td><td>&lt;String></td><td>Read-write</td><td>Schedule export csv_mapping_id.<br>Maximum length = 32</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[ADD]()| [DELETE](#d)| [GET (ALL)](#get-)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###add



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/csv_export?onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/csv_export/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/csv_export
<b>HTTP Method:</b>null
<b>Response Payload: </b>


