
**Usage:** ./HappyCoind [command-line options]

```
Options:
  -?                     This help message
  -conf=<file>           Specify configuration file (default: HappyCoin.conf)
  -pid=<file>            Specify pid file (default: HappyCoind.pid)
  -datadir=<dir>         Specify data directory
  -wallet=<file>         Specify wallet file (within data directory)
  -dbcache=<n>           Set database cache size in megabytes (default: 25)
  -dblogsize=<n>         Set database disk log size in megabytes (default: 100)
  -timeout=<n>           Specify connection timeout in milliseconds (default: 5000)
  -proxy=<ip:port>       Connect through socks proxy
  -socks=<n>             Select the version of socks proxy to use (4-5, default: 5)
  -tor=<ip:port>         Use proxy to reach tor hidden services (default: same as -proxy)
  -torname=<host.onion>  Send the specified hidden service name when connecting to Tor nodes (default: none)
  -dns                   Allow DNS lookups for -addnode, -seednode and -connect
  -port=<port>           Listen for connections on <port> (default: 12846 or testnet: 17778)
  -maxconnections=<n>    Maintain at most <n> connections to peers (default: 125)
  -addnode=<ip>          Add a node to connect to and attempt to keep the connection open
  -connect=<ip>          Connect only to the specified node(s)
  -seednode=<ip>         Connect to a node to retrieve peer addresses, and disconnect
  -externalip=<ip>       Specify your own public address
  -onlynet=<net>         Only connect to nodes in network <net> (IPv4, IPv6 or Onion)
  -discover              Discover own IP address (default: 1 when listening and no -externalip)
  -irc                   Find peers using internet relay chat (default: 1)
  -listen                Accept connections from outside (default: 1 if no -proxy or -connect)
  -bind=<addr>           Bind to given address. Use [host]:port notation for IPv6
  -dnsseed               Find peers using DNS lookup (default: 0) {1)?}
  -cppolicy              Sync checkpoints policy (default: strict)
  -banscore=<n>          Threshold for disconnecting misbehaving peers (default: 100)
  -bantime=<n>           Number of seconds to keep misbehaving peers from reconnecting (default: 86400)
  -maxreceivebuffer=<n>  Maximum per-connection receive buffer, <n>*1000 bytes (default: 5000)
  -maxsendbuffer=<n>     Maximum per-connection send buffer, <n>*1000 bytes (default: 1000)
  -detachdb              Detach block and address databases. Increases shutdown time (default: 0)
  -memorylog             Use in-memory logging for block index database (default: 1)
  -paytxfee=<amt>        Fee per KB to add to transactions you send
  -mininput=<amt>        When creating transactions, ignore inputs with value less than this (default: 0.001)
  -server                Accept command line and JSON-RPC commands
  -testnet               Use the test network
  -debug                 Output extra debugging information. Implies all other -debug* options
  -debugnet              Output extra network debugging information
  -logtimestamps         Prepend debug output with timestamp
  -shrinkdebugfile       Shrink debug.log file on client startup (default: 1 when no -debug)
  -printtoconsole        Send trace/debug info to console instead of debug.log file
  -printtodebugger       Send trace/debug info to debugger
  -rpcuser=<user>        Username for JSON-RPC connections
  -rpcpassword=<pw>      Password for JSON-RPC connections
  -rpcport=<port>        Listen for JSON-RPC connections on <port> (default: 12847 or testnet: 18345)
  -rpcallowip=<ip>       Allow JSON-RPC connections from specified IP address
  -rpcconnect=<ip>       Send commands to node running on <ip> (default: 127.0.0.1)
  -blocknotify=<cmd>     Execute command when the best block changes (%s in cmd is replaced by block hash)
  -walletnotify=<cmd>    Execute command when a wallet transaction changes (%s in cmd is replaced by TxID)
  -confchange            Require a confirmations for change (default: 0)
  -upgradewallet         Upgrade wallet to latest format
  -keypool=<n>           Set key pool size to <n> (default: 100)
  -rescan                Rescan the block chain for missing wallet transactions
  -zapwallettxes         Clear list of wallet transactions (diagnostic tool; implies -rescan)
  -salvagewallet         Attempt to recover private keys from a corrupt wallet.dat
  -checkblocks=<n>       How many blocks to check at startup (default: 2500, 0 = all)
  -checklevel=<n>        How thorough the block verification is (0-6, default: 1)
  -par=N                 Set the number of script verification threads (1-16, 0=auto, default: 0)
  -loadblock=<file>      Imports blocks from external blk000?.dat file

Block creation options:
  -blockminsize=<n>      Set minimum block size in bytes (default: 0)
  -blockmaxsize=<n>      Set maximum block size in bytes (default: 250000)
  -blockprioritysize=<n> Set maximum size of high-priority/low-fee transactions in bytes (default: 27000)

SSL options: (see the Bitcoin Wiki for SSL setup instructions)
  -rpcssl                                  Use OpenSSL (https) for JSON-RPC connections
  -rpcsslcertificatechainfile=<file.cert>  Server certificate file (default: server.cert)
  -rpcsslprivatekeyfile=<file.pem>         Server private key (default: server.pem)
  -rpcsslciphers=<ciphers>                 Acceptable ciphers (default: TLSv1+HIGH:!SSLv2:!aNULL:!eNULL:!AH:!3DES:@STRENGTH)

UI options:
  -lang=<lang>           Set language, for example "de_DE" (default: system locale)
  -min                   Start minimized
  -splash                Show splash screen on startup (default: 1)

```