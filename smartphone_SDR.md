# Modern Smartphone as Software Defined Radio

Can the average smartphone be used as a Software Defined Radio, potentially connecting to networks like LoRA, meshtastic, HAM networks etc, without using external network cards (RTL-SDR for e.g.) 

Notes and links.


## intuition

They should be capable, seeing that some wifi standards (802.11ah/f) were sub Ghz and had support on mobile phones. 

Still, most example projects pursuing this idea use external network cards to achieve the same. 

Obvious reason must be because of the lock in proprietery hardware and software on smartphones, making it non trivial for independent developers to create something like this. Also, tbf, they probably were not intentionally designed and developed for this purpose anyway. 

## promising directions

- https://www.afcea.org/signal-media/smartphones-become-smart-radios
    - abs: Researchers at the Communications Research Centre Canada have proved the feasibility of running public-safety Joint Tactical Radio Network Software Communications Architecture on mobile devices. They successfully accessed three different first-responder frequencies with less modification and effort than expected.

- https://en.wikipedia.org/wiki/IEEE_802.11ah
    - abs: A benefit of 802.11ah is extended range, making it useful for rural communications and offloading cell phone tower traffic. The other purpose of the protocol is to allow low rate 802.11 wireless stations to be used in the sub-gigahertz spectrum.

- https://radiofidelity.com/smart-phones-and-shortwave-radios/
## links

- Electronics Stack Exchnange discussion
    - https://electronics.stackexchange.com/questions/563207/what-exactly-prevents-my-smartphone-from-being-used-as-an-sdr-without-a-dedicate

- [Yotube: RTL-SDR on Android with free software](https://www.youtube.com/watch?v=FgKy9Ffh_aw)

- RTL-SDR
    - https://www.rtl-sdr.com/rtl-sdr-quick-start-guide/
    - https://github.com/shuyuan-liu/sdr-tutorials
    - https://austinsnerdythings.com/2021/09/11/getting-started-with-sdr-software-defined-radio-a-tutorial/

- http://websdr.ewi.utwente.nl:8901/
    - description:  Wide-band WebSDR; On this page you can listen to and control a short-wave receiver located at the amateur radio club ETGD at the University of Twente. In contrast to other web-controlled receivers, this receiver can be tuned by multiple users simultaneously, thanks to the use of Software-Defined Radio.

## Motivation

Abiility to use off grid p2p mesh networks, using average smartphones without dedicated hardware.

Dreams and visions of connecting to long range communication networks in the absence of cellular service. Think initiatives like Meshtastic and other p2p networks, using smartphones that people already have in their hands.

For grokking and giggles. 

Also, relevant if society collapses during my lifetime lol (think hostile aliens, "AGI" takeover, bioweapon leaks, climate disaster etc etc) and I need to survive in the outside (read: not enough money for private self sustaining land and bunker)