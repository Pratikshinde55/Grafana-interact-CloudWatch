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


## Grafana interact with aws:

Grafana nither collect data nor store data, Grafana feedig or taking data from Data Source.

AWS cloud have their own "CloudWatch" for collecting metrics.

Now, we connect grafana to CloudWatch Data Source".

Step 1: Add new data source as Cloud fwatch.

On Grafana WebUI go to "Connections"  Here we see "Add new Data Source" -->> Search and select "Cloud Watch".

![image](https://github.com/user-attachments/assets/2bca37d2-b7db-48d6-a107-4f1e4b5472e6)


Step 2: Authentication Create IAM user 

Now we need Authentication to access aws Cloud Watch, so select access key & secreate key.

- For this i create IAM user on aws console. 

![image](https://github.com/user-attachments/assets/826e2ebd-c840-4558-abb8-04007896f2fa)

- Create Key for "Third-party service"

![image](https://github.com/user-attachments/assets/13343943-4204-44d4-9e1f-a5996ddfb7fc)

- Now Fill/paste key

![image](https://github.com/user-attachments/assets/640e05d4-8b4e-464c-bb38-8ec88e1213d2)

Step 3:


     
