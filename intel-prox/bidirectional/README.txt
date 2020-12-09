Setup
--------------------------------
2 machines are available to run throughput scenario
Parameters:
port1_mac : Mac of Port of Machine 1
port2_mac : Mac of Port of Machine 2


Running PROX commands
------------
Run the following command on machine 1
./build/prox -f machine_1_bidirectional.cfg -w port1_mac=<port1_mac> -w port2_mac=<port2_mac>

Run the following command on machine 2
./build/prox -f machine_2_bidirectional.cfg -w port1_mac=<port1_mac> -w port2_mac=<port2_mac>

Sample PROX commands
------------
./build/prox -f machine_1_bidirectional.cfg -w port1_mac=3c:fd:fe:c1:cf:ec -w port2_mac=3c:fd:fe:c2:23:24
./build/prox -f machine_2_bidirectional.cfg -w port1_mac=3c:fd:fe:c1:cf:ec -w port2_mac=3c:fd:fe:c2:23:24
