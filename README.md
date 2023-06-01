# elasticsearch-demo

following the tutorial ["Beginners crash course to Elastic Stack"](https://youtu.be/gS_nHTWZEJ8)

installation instructions that worked for me: 
- download elasticsearch and kibana archives, unzip them
- run `cd elasticsearch && bin/elasticsearch`, keep the terminal tab open
- check the connection with `curl --cacert http_ca.crt -u elastic https://localhost:9200`
- `cd kibana && bin/kibana` in a separate tab, keep open as well
- to login into kibana change the password using `bin/elasticsearch-reset-password --username kibana_system`
- go to http://localhost:5601/ and choose the login option using the login/password
- then change the password to elastic user using the previous command or use the password printed on the elastic tab to login into elastic
- after successful login go to the left menu -> managment -> dev tools

if anything goes wrong, try reinstalling elasticsearch/kibana by deleting the folder and unziping the acrhive again
