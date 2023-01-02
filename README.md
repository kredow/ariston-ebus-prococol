Ariston BridgeNet protocol is based on eBUS specification but with extended application layer.
It introduces new PSBS commands and own communication model.  

It seems that devices communicate by accessing registers like a virtual memory map of the system.
New commands used by protocol PBSB:  
- 2000, 2001
  - direct reads of the registers i.e. 313c2000020120 / 020101
  - broadcast reads of a single register

- 200e, 200f, 2010, 2020
  - broadcast responses for 2000 request
  - broadcasts with multiple register values i.e. 37fe20101002910000039100000491000005910000

Some of them are less commonly used like
2050
2051
2071
2073







