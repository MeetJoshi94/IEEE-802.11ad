# IEEE-802.11ad
ns3 simulations of IEEE 802.11ad
hdrelaybuilding.cc : 
Modified version of the code 'evaluate_halfduplex_relay_tcp.cc' by Hany Assasa.  
Instead of FrissPropagationLossModel, OhBuildingsPropagationLossModel is used.
Flow monitor tool is also added to the code.
To use OhBuildingsPropagationLossModel nodes need to have positive z coordinates. It will give some error if nodes are placed on the dimension loke(x,y,0).

Build the ns3 by using the following command.
CXXFLAGS="-Wall" ./waf configure --disable-examples --disable-tests --disable-python --enable-modules='applications','core','internet','point-to-point','wifi','buildings','flow-monitor'
