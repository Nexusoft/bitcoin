Let us not forget our roots, Bitcion v0.1.0. Pure code as close to Satoshi as you can get.
We have this pinned to our organization to remind everyone where we came from, so that we
can better see where we are going.

Announcement
-----
Announcing the first release of Bitcoin, a new electronic cash
system that uses a peer-to-peer network to prevent double-spending.
It's completely decentralized with no server or central authority.

See bitcoin.org for screenshots.

Download link:
http://downloads.sourceforge.net/bitcoin/bitcoin-0.1.0.rar

Windows only for now. Open source C++ code is included.

- Unpack the files into a directory
- Run BITCOIN.EXE
- It automatically connects to other nodes

If you can keep a node running that accepts incoming connections,
you'll really be helping the network a lot. Port 8333 on your
firewall needs to be open to receive incoming connections.

The software is still alpha and experimental. There's no guarantee
the system's state won't have to be restarted at some point if it
becomes necessary, although I've done everything I can to build in
extensibility and versioning.

You can get coins by getting someone to send you some, or turn on
Options->Generate Coins to run a node and generate blocks. I made
the proof-of-work difficulty ridiculously easy to start with, so
for a little while in the beginning a typical PC will be able to
generate coins in just a few hours. It'll get a lot harder when
competition makes the automatic adjustment drive up the difficulty.
Generated coins must wait 120 blocks to mature before they can be
spent.

There are two ways to send money. If the recipient is online, you
can enter their IP address and it will connect, get a new public
key and send the transaction with comments. If the recipient is
not online, it is possible to send to their Bitcoin address, which
is a hash of their public key that they give you. They'll receive
the transaction the next time they connect and get the block it's
in. This method has the disadvantage that no comment information
is sent, and a bit of privacy may be lost if the address is used
multiple times, but it is a useful alternative if both users can't
be online at the same time or the recipient can't receive incoming
connections.

Total circulation will be 21,000,000 coins. It'll be distributed
to network nodes when they make blocks, with the amount cut in half
every 4 years.

first 4 years: 10,500,000 coins
next 4 years: 5,250,000 coins
next 4 years: 2,625,000 coins
next 4 years: 1,312,500 coins
etc...

When that runs out, the system can support transaction fees if
needed. It's based on open market competition, and there will
probably always be nodes willing to process transactions for free.

Satoshi Nakamoto


Intro
-----
Bitcoin is an electronic cash system that uses a peer-to-peer network to
prevent double-spending.  It's completely decentralized with no server or
central authority.


Operating Systems
-----------------
Windows NT/2000/XP (and probably Vista)

Vista hasn't been tested yet.  All the libraries used are cross-platform, so
there's nothing preventing future Linux and Mac builds.


Setup
-----
Unpack the files into a directory and run bitcoin.exe.

The software automatically finds other nodes to connect to.  You should set
your firewall to forward port 8333 to your computer so you can receive incoming
connections, otherwise the nodes you can connect with will be limited.

To support the network by running a node, select:

  Options->Generate Coins

and keep the program open or minimized.  It runs at idle priority when no other
programs are using the CPU.  Your computer will be solving a very difficult
computational problem that is used to lock in blocks of transactions.  The time
to generate a block varies each time, but may take days or months, depending
on the speed of your computer and the competition on the network.  It's not a
computation that has to start over from the beginning if you stop and restart
it.  A solution might be found at any given moment it's running.  As a reward
for supporting the network, you receive coins when you successfully generate a
block.
