# Grafana-interact-CloudWatch
Grafana interact with aws CloudWatch data source

Grafana is open-source software tool that helps user visualize, query, and understand data.

Grafana capture data from all services and give "Single pane of glass" view.

Grafana give entire visibilty stack.

Grafana create visuale on the to of "Metrics","logs","Traces".

Grafana is powerfull in Metrics perspective.


### How to download grafana:

I use aws instance for download grafana (AMI- amazon linux 2)

Search on google grafana download for linux and download Standalone Linux Binaries 64 Bit tar file. 
(Link:-  https://grafana.com/grafana/download )

Command for download grafana:

     wget https://dl.grafana.com/enterprise/release/grafana-enterprise-11.2.0.linux-amd64.tar.gz

Command for Extract Grafana:

     tar -zxvf grafana-enterprise-11.2.0.linux-amd64.tar.gz

Now start Grafana server:

     ./grafana-server &

![image](https://github.com/user-attachments/assets/1beff168-7444-468c-9d99-fa8963d54a48)

     
- Note:

Grafana work on port no 3000.

Grafana work on "Http" protocol.


##### Connect grafana webUI;

Now connect to grafana by webUI --->>  Public Ip:port no (http://43.204.97.131:3000)

- Note:

Edit Inbound rule of grafana instance: (Enable port 3000 to my IP)

![image](https://github.com/user-attachments/assets/e817b3ca-15ba-42f0-8537-76821b176cbe)

Grafana WEbUI:
![image](https://github.com/user-attachments/assets/540075e2-e041-41f2-bdf3-feb1df5fd828)


     
