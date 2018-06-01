#ldap_server

Configuration for LDAP Server resource.


##Properties 
<span>(click to see [Operations](#opera))</span>


<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>auth_timeout</td><td>&lt;Integer></td><td>Read-write</td><td>The maximum number of seconds the system will wait for a response from the LDAP server.</td></tr><tr><td>group_search_subattribute</td><td>&lt;String></td><td>Read-write</td><td>LDAP group search subattribute. Used to determine to which groups a group belongs..<br>Maximum length = 32</td></tr><tr><td>follow_referrals</td><td>&lt;Boolean></td><td>Read-write</td><td>Enable following LDAP referrals received from LDAP server.</td></tr><tr><td>search_filter</td><td>&lt;String></td><td>Read-write</td><td>The String to be combined with the default LDAP user search string to form the value.<br>Maximum length = 256</td></tr><tr><td>group_attr_name</td><td>&lt;String></td><td>Read-write</td><td>The Attribute name for group extraction from the LDAP server.<br>Maximum length = 32</td></tr><tr><td>authentication</td><td>&lt;Boolean></td><td>Read-write</td><td>Set to false for public key Authentication.</td></tr><tr><td>ldap_host_name</td><td>&lt;String></td><td>Read-write</td><td>Host Name on the certificate from LDAP Server.<br>Maximum length = 128</td></tr><tr><td>change_password</td><td>&lt;Boolean></td><td>Read-write</td><td>Enable change of the user.</td></tr><tr><td>default_authentication_group</td><td>&lt;String></td><td>Read-write</td><td>This is the default group.<br>Maximum length = 64</td></tr><tr><td>max_nesting_level</td><td>&lt;Integer></td><td>Read-write</td><td>Number of levels at which group extraction is allowed.<br>Maximum value =</td></tr><tr><td>login_name</td><td>&lt;String></td><td>Read-write</td><td>The name attribute used by the system to query the external LDAP server.<br>Maximum length = 32</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the ldap servers.</td></tr><tr><td>ip_address</td><td>&lt;String></td><td>Read-write</td><td>The IP address of the LDAP server..<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>nested_group_extraction</td><td>&lt;Boolean></td><td>Read-write</td><td>Enable Nested Group Extraction.</td></tr><tr><td>group_search_attribute</td><td>&lt;String></td><td>Read-write</td><td>LDAP group search attribute. Used to determine to which groups a group belongs.<br>Maximum length = 32</td></tr><tr><td>ssh_public_key</td><td>&lt;String></td><td>Read-write</td><td>SSH public key attribute holds the public keys of the user.<br>Maximum length = 64</td></tr><tr><td>group_name_identifier</td><td>&lt;String></td><td>Read-write</td><td>Name that uniquely identifies a group in LDAP server.<br>Maximum length = 32</td></tr><tr><td>subattribute_name</td><td>&lt;String></td><td>Read-write</td><td>The Sub-Attribute name for group extraction from LDAP server.<br>Maximum length = 32</td></tr><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Name of LDAP server.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>validate_ldap_server_certs</td><td>&lt;Boolean></td><td>Read-write</td><td>Validate LDAP Server Certificate.</td></tr><tr><td>group_search_filter</td><td>&lt;String></td><td>Read-write</td><td>String to be combined with the default LDAP group search string to form the search value.<br>Maximum length = 128</td></tr><tr><td>bind_dn</td><td>&lt;String></td><td>Read-write</td><td>The full distinguished name used to bind to the LDAP server.<br>Maximum length = 128</td></tr><tr><td>port</td><td>&lt;Integer></td><td>Read-write</td><td>The port number on which the LDAP server is running.<br>Maximum value =</td></tr><tr><td>base_dn</td><td>&lt;String></td><td>Read-write</td><td>The base or node where the ldapsearch should start.<br>Maximum length = 128</td></tr><tr><td>sec_type</td><td>&lt;String></td><td>Read-write</td><td>The communication type between the system and the LDAP server.</td></tr><tr><td>max_ldap_referrals</td><td>&lt;Integer></td><td>Read-write</td><td>Maximum number of ldap referrals to follow.</td></tr><tr><td>type</td><td>&lt;String></td><td>Read-write</td><td>The type of LDAP server.<br>Minimum length = 2<br>Maximum length = 64</td></tr><tr><td>bind_passwd</td><td>&lt;String></td><td>Read-write</td><td>The password used to bind to the LDAP server.<br>Maximum length = 128</td></tr><tr><td>address_type</td><td>&lt;Integer></td><td>Read-only</td><td>Configuration Type. Values: 0: IPv4, 1: IPv6, -1: Hostname.</td></tr></tbody></table>
##Operations 
<span>(click to see [Properties](#prope))</span>


[ADD]()| [DELETE](#d)| [GET (ALL)](#get-)| [GET]()| [UPDATE](#u)


Some options that you can use for each operations:
<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note:</b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>



***Note:*** 
Mandatory parameters are marked in <span style="color:#FF0000;">red</span>and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.

###add



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ldap_server?onerror=&lt;String_value&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>



###delete



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ldap_server/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get (all)



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ldap_server
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###get



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ldap_server/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Response Payload: </b>



###update



<b>URL:</b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ldap_server/id_value&lt;String&gt;
<b>HTTP Method:</b>null
<b>Request Payload: </b>
<b>Response Payload: </b>


