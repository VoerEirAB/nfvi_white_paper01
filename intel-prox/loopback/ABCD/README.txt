Setup
--------------------------------
2 machines are available to run throughput scenario
Parameters:
sender_mac : Mac of TX Port of sender/receiver machine
receiver_mac : Mac of RX Port of sender/receiver machine
rx_reflector_mac : Mac of RX Port  of reflector machine
tx_reflector_mac : Mac of TX Port of reflector machine


Running PROX commands
------------
Run the following command on machine 1
./build/prox -f reflector_loopback_abcd.cfg -w rx_reflector_mac=<rx_reflector_mac> -w tx_reflector_mac=<tx_reflector_mac> -w receiver_mac=<receiver_mac>

Run the following command on machine 2
./build/prox -f sender_receiver_abcd_loopback.cfg -w sender_mac=<sender_mac> -w receiver_mac=<receiver_mac> -w rx_reflector_mac=<rx_reflector_mac>

Sample PROX commands
------------
./build/prox -f reflector_loopback_abcd.cfg -w rx_reflector_mac=3c:fd:fe:c1:b6:11 -w tx_reflector_mac=3c:fd:fe:c2:04:5d -w receiver_mac=3c:fd:fe:c1:cf:b1
./build/prox -f sender_receiver_abcd_loopback.cfg -w sender_mac=3c:fd:fe:c1:b5:85 -w receiver_mac=3c:fd:fe:c1:cf:b1 -w rx_reflector_mac=3c:fd:fe:c1:b6:11