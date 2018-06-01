#mps_datacenter

Configuration for MPS Datacenter resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>country</td><td>&lt;String></td><td>Read-write</td><td>country.<br>Maximum length = 32</td></tr><tr><td>longitude</td><td>&lt;Double></td><td>Read-write</td><td>longitude of the city.</td></tr><tr><td>is_default</td><td>&lt;Boolean></td><td>Read-write</td><td>IS Default Datacentre.</td></tr><tr><td>location</td><td>&lt;String></td><td>Read-write</td><td>Cloud Provide.</td></tr><tr><td>region</td><td>&lt;String></td><td>Read-write</td><td>region.<br>Maximum length = 64</td></tr><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Datacentre Name.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>zipcode</td><td>&lt;String></td><td>Read-write</td><td>Zipcode of location.<br>Maximum length = 32</td></tr><tr><td>cloud_vpc</td><td>&lt;String></td><td>Read-write</td><td>cloud_vpc.<br>Maximum length = 64</td></tr><tr><td>city</td><td>&lt;String></td><td>Read-write</td><td>city.<br>Maximum length = 64</td></tr><tr><td>tenant_id</td><td>&lt;String></td><td>Read-write</td><td>Tenant ID.</td></tr><tr><td>cloud_provider</td><td>&lt;String></td><td>Read-write</td><td>Cloud Provide.</td></tr><tr><td>latitude</td><td>&lt;Double></td><td>Read-write</td><td>latitude of the city.</td></tr><tr><td>cloud_region</td><td>&lt;String></td><td>Read-write</td><td>cloud_region.<br>Maximum length = 64</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the system users.</td></tr><tr><td>type</td><td>&lt;Integer></td><td>Read-write</td><td>Datacenter type: Site/Datacenter.</td></tr><tr><td>count_map</td><td>&lt;entity_map[]></td><td>Read-write</td><td>Count Map.</td></tr><tr><td>application_name</td><td>&lt;String></td><td>Read-write</td><td>Application Name.</td></tr><tr><td>device_ip</td><td>&lt;String></td><td>Read-write</td><td>Device Ip.</td></tr><tr><td>total_critical_events</td><td>&lt;Integer></td><td>Read-only</td><td>Total Critical events city wise..</td></tr><tr><td>total_number_of_devices</td><td>&lt;Integer></td><td>Read-only</td><td>Total number of devices deployed city wise...</td></tr><tr><td>total_major_events</td><td>&lt;Integer></td><td>Read-only</td><td>Total major events..</td></tr><tr><td>total_events</td><td>&lt;Integer></td><td>Read-only</td><td>Total events city wise..</td></tr><tr><td>total_number_of_agents</td><td>&lt;Integer></td><td>Read-only</td><td>Total number of agents deployed city wise..</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[ADD]()| [DELETE](#d)| [GET (ALL)](#get-)| [GET]()| [UPDATE](#u)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###add



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_datacenter?onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_datacenter/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_datacenter
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_datacenter/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###update



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/mps_datacenter/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>


