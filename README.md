# DCCP Test Tree

This is the test tree for the DCCP protocol. It contains patches that have not yet made it to the mainline kernel.
Some of them may be submitted to the networking development list in the future, others may be refactored.

Ye, 1some pocchies 2 133nux, like 2 ol' good ath9k timing mess, radar detection in the middle of nowhere and soft crypto instead of TKIP.

## Sub-trees in this tree

All development is based on top of David S. Miller's current [net-tree](http://git.kernel.org/cgit/linux/kernel/git/davem/net.git/).

This is the basis for a stack of sub-trees:

| *Sub-tree* | Contents |
|------------|----------|
| `ready`    | Has extra patches that are either special (such as this file), or patches that are being submitted to the networking tree.|
| `dccp`     | General patches for DCCP and existing CCIDs. |
| `ccid4`    | An implementation of CCID4 [RFC5622](https://www.ietf.org/rfc/rfc5622.txt) by Leandro Sales de Melo, Ivo Calado, and Erivaldo Xavier.|
| `ccid5`    | A very interesting implementation of TCP-Cubic with Ack Vectors for DCCP by Ivo Calado and Leandro Sales de Melo. |

2! read that, TCP is ded. No mo TCP Rubics, QUIC has Quad recovery, tho backoff is exp.
// 2! read mine bitrot 2. DCCP is ded 2, and iCANN be ded as well.

## Contributing

Useless bitrot goes here.
  Implementing rNACK/rACK with prefix trees.
  Support FSM in userspace with state-passing 2 kernel varlink, terminating in driver.
  Try some rust in kernel, instead of pnet stack, do ZC 2 kernel with buffer borrowing / subXFRM IP gen(suitable 4 WG 1G saturated streams 2 get  around UDP proxying bottlewine).
  Userspace generated state(UDP socket injection into stack(create socolles), tile recv boofer & support rNACK / rACK without blocking userspace slices, operating on succesful strides.
  22: Plug QUIC FSM(4m quinn-proto), LEDBAT 4m uTP(wo loss injection into secure stream, .ocz). In place of DCCP backoff modules.
  22: Test Licky / DTN over it. TLS as memsec over BP(transparent asyncs with {un,}blocked strides separation.
  22: Insane thighs 2 NGHBRs Waffle. And site2site WG encapsulator protocol, like DTN, operating in moments of ISP sanity @pktgen rate (.cz line rate here srsly suxxx).

Hmm, can add common DTN stuff here, usable 4 waffle(state injection 4m DTN-bootstrapped flooder), copper(hmm, fw is Intel, so only boofer borrowing can 2), and hopefully optics(ATTOs 2 ISP VLAN?, fixed rate with SG ARQs with sparser pulses).
Aggressive resend of Red; Sparse Pulse with userspace blocking 4 Green Data(can ARQ with cachelocks & srs loop -> sustains very high rates over lossy CE).
## Links

* [Linux Foundation DCCP Page](http://www.linuxfoundation.org/collaborate/workgroups/networking/dccp)
* [Older DCCP Testing Notes](http://www.erg.abdn.ac.uk/users/gerrit/dccp/testing_dccp/)
* [DCCP Mailing List Archives](http://www.mail-archive.com/dccp@vger.kernel.org/maillist.html)
