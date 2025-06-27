<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle Examples</h1>
This walkthrough involves creating tickets as end users. We will then observe all the ticket properties and respond to them as help desk professionals. This builds upon the previous project: osTicket: Post-Installation Configuration.<br />


<h2>Environments Used</h2>

- Microsoft Azure
- macOS (Host Machine)
- Windows 10
- Windows App (Remote Desktop)

<h2>Technology/Applications/Services </h2>

- osTicket
- Azure Virtual Machines




<h2>Walkthrough</h2>

</br>
<h3 align="center">
  Let’s create our first ticket as an end user
</h3>
</br>

As an end user named Karen, we create a ticket</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Issue: Banking System Down

  
![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic1.png)
</p>
<br />
<p>
As a Help Desk Agent (John), observe the ticket’s properties(ex. Priority, Department, SLA, Assigned To)
  

![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic2.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic3.png)

<br />

<p>
Set Properties to the ticket<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- SLA Plan: Sev-A (1 hour, 24/7)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Help topic: Business Critical Outage<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Assign to: Online Banking <br />
*Each of these updates show up in the tickets thread for the agents to see(not the end-user) 


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic4.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic5.png)

<br />




![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic6.png)
</p>
<br />
<p>
We can even log in as Help Desk Agent Jane and work the ticket to completion.
</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic7.png)

<br />

<p>
As Jane we can assign the ticket to ourselves. This can be good practice as it lets John and other agents know that they can focus on another ticket.
</p>


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic8.png)
</p>
<br />
<p>
Even if the complete solution isn’t found, it is good, maybe even a requirement in some companies to provide the end user with updates like the following.(In most ticketing systems, users receive an email when there’s an update.)
</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic9.png)
</p>
<br />
<p>
We found the solution.

  
</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic10.png)
</p>
<br />
<p>
Since the problem is solved, by clicking the ticket’s “Status:”, we can change the status to Resolved instead of Open.
</p>

![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic11.png)
</p>
<br />
<p>
And with the previous step, the ticket is removed from the list of tickets. So agents can focus on other ongoing tickets or if empty, they can be ready for future tickets.
</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic12.png)
</p>
<br />
<p>
As an admin or an agent with a lot of permissions, you can still view tickets that have been closed.
Admin/Agent Panel -> Tickets -> Closed


</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic13.png)

<br />

<p>
  <h3 align="center">
Now let’s solve another ticket.<br />
  </h3>
As an end user named Ken, we create a ticket.<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Issue: Use of Adobe Software 
</p>


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic14.png)
</p>
<br />

<p>
*Let's say we had a phone call with Ken. He says only 2 people in the accounting department are having difficulty with using the software. This is key information in determining the SLA Plan for the ticket. We pick plan C instead of A or B.
</p>

<br />

<p>
As a Help Desk Agent (John), we will resolve the ticket.<br />
Set Properties to the ticket<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- SLA Plan: Sev-C (8 hours, 24/5)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Help topic: General Inquiry/Other<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Assign to: Support/John Doe(myself) 
 </p>


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic15.png)
</p>
<br />

<p>
In a phone call, we tell Ken that the 2 people in the accounting department should restart their computer to solve the issue, since there were a lot of updates yesterday. Ken will call us back after lunch to let us know if it worked. We should make an update of this on osTicket like the following. 
</p>


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic16.png)
</p>
<br />
<p>
On a phone call after lunch, Ken tells us restarting made it work. We update once again and close the ticket like we’ve done before.
</p>



![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic17.png)
</p>
<br />

<h3 align="center">
  *TIPS
</h3>

<br />

<p>
In the previous ticket a lot of communication happened via phone call. In some cases, the issue from the start may be introduced through phone, chat app, email, web form, or maybe even you run into someone in your hall or they come to your desk.
</p>
<br />
<p>
It is good practice to still create a ticket for this, even if you can solve the issue on the spot.
Agent Panel -> Tickets -> New Ticket
</p>


![image alt](https://github.com/GursimarJ/ticket-lifecycle/blob/3db9f56b7a9d2057f6f980176affb5b7befca8d6/assets/Part3Pic18.png)
