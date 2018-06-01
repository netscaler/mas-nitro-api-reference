#haproxy_frontend_stats

Configuration for HAProxy frontend stats information resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>bin</td><td>&lt;Double></td><td>Read-write</td><td>Bytes of date in.</td></tr><tr><td>hrsp_1xx</td><td>&lt;Double></td><td>Read-write</td><td>No of request with response code 1XX.</td></tr><tr><td>bout</td><td>&lt;Double></td><td>Read-write</td><td>Bytes of data out.</td></tr><tr><td>hrsp_other</td><td>&lt;Double></td><td>Read-write</td><td>No of request with other response code.</td></tr><tr><td>dresp</td><td>&lt;Double></td><td>Read-write</td><td>No of response denied.</td></tr><tr><td>scur</td><td>&lt;Double></td><td>Read-write</td><td>Current Session.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key.</td></tr><tr><td>hrsp_2xx</td><td>&lt;Double></td><td>Read-write</td><td>No of request with response code 2XX.</td></tr><tr><td>dreq</td><td>&lt;Double></td><td>Read-write</td><td>No of denied requests.</td></tr><tr><td>frontend_id</td><td>&lt;String></td><td>Read-write</td><td>Frontend ID.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>svname</td><td>&lt;String></td><td>Read-write</td><td>Service Name.<br>Minimum length = 1<br>Maximum length = 100</td></tr><tr><td>hrsp_4xx</td><td>&lt;Double></td><td>Read-write</td><td>No of request with response code 4XX.</td></tr><tr><td>hrsp_3xx</td><td>&lt;Double></td><td>Read-write</td><td>No of request with response code 3XX.</td></tr><tr><td>hrsp_5xx</td><td>&lt;Double></td><td>Read-write</td><td>No of request with response code 5XX.</td></tr><tr><td>req_rate</td><td>&lt;Double></td><td>Read-only</td><td>HTTP Reqrate/Sec.</td></tr><tr><td>ereq</td><td>&lt;String></td><td>Read-only</td><td>Number of error requests.</td></tr><tr><td>req_tot</td><td>&lt;String></td><td>Read-only</td><td>Total number of requests.</td></tr><tr><td>eresp</td><td>&lt;String></td><td>Read-only</td><td>Number of error responses.</td></tr><tr><td>stot</td><td>&lt;Double></td><td>Read-only</td><td>Total number of sessions.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[GET (ALL)](#get-)| [GET]()


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/haproxy_frontend_stats
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/haproxy_frontend_stats/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>


