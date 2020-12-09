Setup
--------------------------------
2 machines are available to run throughput scenario
Parameters:
src_mac : Mac of Port of sender/receiver machine
dst_mac : Mac of Port of reflector machine


Running PROX commands
------------
Run the following command on machine 1
./build/prox -f reflector_loopback_aba.cfg -w dst_mac=<reflector_port_mac>

Run the following command on machine 2
./build/prox -f sender_receiver_ABA_loopback.cfg -w dst_mac=<reflector_port_mac> -w src_mac=<sender_port_mac>

Sample PROX commands
------------
./build/prox -f reflector_loopback_aba.cfg -w dst_mac=3c:fd:fe:c2:23:24
./build/prox -f sender_receiver_ABA_loopback.cfg -w dst_mac=3c:fd:fe:c2:23:24 -w src_mac=3c:fd:fe:c1:cf:ec
