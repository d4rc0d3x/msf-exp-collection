# Exploits Collection
Exploits in general (metasploit packs, metasploit, custom, third party, etc)

The exploits in this repository are a collection of WORKING exploits gathered throught the Internet during a long time from all kinds of sources such as:

# Current Metasploit State

```
+ -- --=[ 1545 exploits - 950 auxiliary - 264 post        ]
+ -- --=[ 438 payloads - 38 encoders - 8 nops             ]
```

# Metasploit Exploit Packs

The following Metasploit Exploit Packs can be found compiiled here in "msf4-root" directory:

1. Metasploit
2. Viproy (http://www.viproy.com/)
3. WPSploit (https://github.com/espreto/wpsploit)
4. MetaSSH (https://github.com/dirtyfilthy/metassh)
5. ... etc

# Exploit Databases

Exploits from the following databases can be found here:

1. Exploit-db (https://www.exploit-db.com/)
2. Vulnerability Lab (http://www.vulnerability-lab.com/)
3. 0day.today (http://0day.today/)
4. PacketStorm (https://packetstormsecurity.com/files/tags/exploit/)
5. CXSecurity (http://cxsecurity.com/)
6. Intelligent Exploit (https://www.intelligentexploit.com/)
7. Exploit-ID (http://www.exploit-id.com/)
8. ExploitHub (https://exploithub.com)

# Installation Instructions

[METASPLOIT EXPLOITS]

Copy the entire content of the "msf4-root" to your ~"/.msf4/modules/" directory


[MODULES CONFIGURATION]

Search for your metasploit modules "mixins.rb" file, generally in "~<msf_root_directory>/lib/msf/core/auxiliary/mixins.rb" 
Include the following entries at the end of the file:

  require '/root/.msf4/modules/lib/msf/core/auxiliary/sip'
  require '/root/.msf4/modules/lib/msf/core/auxiliary/skinny'
  require '/root/.msf4/modules/lib/msf/core/auxiliary/msrp'

[EXPLOITS CONFIGURATION]

Search for your metasploit modules "mixins.rb" file, generally in "~<msf_root_directory>tools/modules/module_mixins.rb" 
Include the following entries at the end of the file:

[FINAL CONFIGURATIONS]

Restart metasploit framework

root:/root# service metasploit restart
