Setup
--------------------------------
2 machines are available to run throughput scenario
Parameters:
sender_mac : Mac of TX Port of sender/receiver machine
receiver_mac : Mac of RX Port of sender/receiver machine


Running PROX commands
------------
Run the following command on machine 1
./build/prox -f receiver_1_core_2_queues.cfg -w receiver_mac=<receiver_mac>

Run the following command on machine 2
./build/prox -f max_generate_sender_1_core_2_queues.cfg -w sender_mac=<sender_mac> -w receiver_mac=<receiver_mac>

Sample PROX commands
------------
./build/prox -f receiver_1_core_2_queues.cfg -w receiver_mac=3c:fd:fe:c1:cf:b1
./build/prox -f max_generate_sender_1_core_2_queues.cfg -w sender_mac=3c:fd:fe:c1:b5:85 -w receiver_mac=3c:fd:fe:c1:cf:b1