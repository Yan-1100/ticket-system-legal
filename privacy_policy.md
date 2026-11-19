**Privacy Policy — Ticket System**  
*Last updated: November 20, 2026.*  
Ticket System ("the Bot", "we") is a support-ticket bot for Discord servers. This policy explains what data the Bot processes, why, and how you can control it. By using the Bot on a Discord server you agree to this policy.  
**1. What data we process**  
**1.1 Server configuration**  
Set by server administrators with `/setup` and `/panel`:  
- Discord IDs of the server, channels, the ticket category, and the moderator/administrator roles configured for each ticket panel;  
- panel settings: panel name, text and colour of the panel message, form field labels, switches (ratings, role ping) and the ID of the panel message.  
**1.2 Tickets (only when you open a ticket)**  
When a member opens a ticket, the Bot:  
- creates a private channel visible to that member, the Bot and the moderators. The channel topic stores technical IDs: the member's ID, the ticket type ID and the ID of the moderator who took the ticket;  
- posts the answers the member typed into the ticket form (subject, description, optional extra answers) in that channel. The subject is also shown in the notification in the staff channel;  
- when the ticket is closed, reads the message history of that ticket channel (author names, message text, embed text) and builds a plain-text transcript. The transcript is sent as a file to the server's staff channel in Discord. It is built in memory and is **not** saved by the Bot in its database or on disk;  
- deletes the ticket channel after the ticket is closed.  
Ticket channel names contain the member's Discord username. This name can appear in messages the Bot posts in the staff channel (closing notice, rating result).  
**1.3 Ratings**  
After a ticket is closed, the member may rate the help (helpful / not helpful, and 1–5 stars). The Bot stores only the server ID, the moderator's ID, whether the help was rated helpful, the number of stars and the time. Ratings are not linked to the member who gave them.  
**1.4 Staff statistics**  
Only for members who hold a moderator or administrator role configured by the server's administrators:  
- number of tickets handled, number of successful tickets, total stars (average rating);  
- number of messages sent (a counter only — the text is not stored);  
- time spent in voice channels;  
- time online (online/offline status only; we do not read activities, games or custom status).  
These values are stored together with the member's Discord ID and the server ID. Messages, voice activity and online status of regular members are not recorded.  
**1.5 What we do not do**  
- We do not store message content in a database. Messages outside ticket channels are received by the Bot only to increase a counter when the author is staff, and are then discarded.  
- We do not collect direct messages, e-mail addresses, IP addresses or payment data.  
- We do not sell data, use it for advertising, or use it to train AI/ML models.  
**2. Why we process it**  
- to run the ticket system (create, claim, close tickets, send transcripts, collect ratings);  
- to show statistics and leaderboards of the server's moderation team (`/stats`, `/rating`);  
- to keep each server's configuration.  
**3. Discord privileged intents**  
- **Server Members** — to see which members hold the configured staff roles and to give a moderator access to a ticket channel;  
- **Message Content** — to build the ticket transcript and to run the admin prefix command used to synchronise slash commands;  
- **Presence** — to measure the online time of staff members only.  
**4. Storage, retention and deletion**  
- Data is stored in a database on the server where the Bot is hosted.  
- Ticket transcripts are not stored by us. They stay in the staff channel in Discord and are subject to that server's rules and Discord's policies.  
- Server configuration and statistics are kept while the Bot is used on the server. If the Bot is removed from a server, its data stays in our database until it is deleted on request.  
- To have data deleted, contact us. We normally act within 30 days.  
**5. Sharing**  
We do not sell or share data with third parties, and cases where the law requires it.  
Statistics shown by `/stats` and `/rating` are visible to the member who runs the command. By default any member of the server can run them. Server administrators can restrict these commands in Discord.  
**6. Your choices**  
- **Members:** you decide whether to open a ticket. By creating a ticket you agree to the terms. The Bot reads message text only in ticket channels.  
- **Staff:** ask your server administrator to remove your staff role from the panel settings to stop new statistics, and contact us to delete the statistics already stored.  
- **Server administrators:** you can change roles or remove the Bot at any time.  
You can contact us with a request to delete all data.  
   
   
 **7. Contact us**  
- helpdsbots@outlook.com  
