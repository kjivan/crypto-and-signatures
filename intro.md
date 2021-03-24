## **Cryptography &</br> Signatures**

Kavi Jivan

Note:
I really liked Frank's intro slides so I'm going to do a quick intro.

---

## Overview

</br>

### Problem

Secure Internet Communication
</br>
Secure = Confidential and Integral(Verified Recipient)

</br>


#### Solution
- Simple -> Complex
- Past -> Present
- Physical -> Digital

Note:
Originally I was going to do the presentation with a greater focus on the history and time line.
However, while working on the presentation I thought it would be better to focus on solving the fundamental 
problem that cryptography and signatures try to solve.
That problem being secure Internet communication! For the purposes of this presentation I'm calling 
secure confidential meaning only you and the recipient understand
and verified as in the identity of the person/organization on the other end of the connection. 
That message is ending up with the right person.
But we are still going to keep some history in there since I want to do a bottom-up building of network security. So we will be working from simple to more complex. This also tends to mean from the past to present
and physical to digital.
Disclaimer: All this stuff is kind of new to me so if you can correct something feel free to do so
and if you have any questions also feel free to raise your hand i'll keep an eye on the chat window.

---
## Internet (1990)

Internet = Connectivity and Communication


![US Night Lights](images/light.jpg)

Photo by [NASA](https://unsplash.com/@nasa?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/internet?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

<!-- HTML comment recognizes as a presenter note per pages. -->
<!-- You may place multiple comments in a single page. -->

Note:
The internet we use today has it's beginnings at CERN Switzerland in 1990 and well we all knew it grew rapidly.
There were some earlier variations that were decommission over time. So what is the internet.
Fundamentally the internet is two things the physical connections between devices and the protocols that allow devices to understand each other.
This allows us and our devices to all communicate with one other. On the connections as you can see in the map not every
place is directly connected to another. This is a critical detail at our attempts at secure communication.

---

## Plain Message over the Internet

</br>
</br>
👩‍💻 --------✉️-------> 🏦

Note:
This is the simplest understanding of the web we can get where we simply send messages from one place to another. In this example from a client of a bank to the bank's website.
This women behind the laptop is logging onto her bank's website and maybe using her login to pay a bill. This is similar to snail mail or physical mailing a letter or check.

---

## Hacker in the Network

</br>
</br>
👩‍💻 -------✉️🦹-------> 🏦

</br>
</br>

🦹📩 = 💸

Note:
So first off, you'll notice the hacker's attire, I don't know what to say. I don't know why hackers dress that way, but they do.
Anyhow, as I mentioned earlier the internet is connected through a network which means it's not going directly from point to point.
It's actually hitting other machines on the way to it's destination and the source connection could also be shared.
WiFi is a notorious example of this since WiFi is not point to point. You can't really restrict radio waves to a person and so anyone can listen in 
on those connections. So if you compare this to snail mail. Snail mail is far less accessible(mostly just USPS). In this case,
the hacker was simply listening in on the connection and just takes your password from the conveniently placed message in their
reach.


---
## Internet Stack

![Protocol Stack](images/stack.svg)

Note: So why did this happen? Well if we look at what the internet is made of from a vertical slice it does not have security built in
to the lower layers of it's architecture. Walk through stack and get to security. This has been a long standing complaint of our current
internet protocol stack. Google engineers have introduced a protocol called QUIC as part of HTTPS3 which pushes security down a layer and
will replace TCP.

--

Image from [wikipedia](https://en.wikipedia.org/wiki/Protocol_stack)
