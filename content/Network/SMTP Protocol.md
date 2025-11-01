#network 
[[Network MOC]]
- - -

The Simple Mail Transfer Protocol is ancient, but too widely used to change easily. It is connection-oriented, like the [[TCP Protocol]]. It is commonly used in [[Email Server|email servers]] for sending email or between e-mail servers.

# Commands

- **MAIL**: Establishes return address, bounce address, sender, and more
- **RCPT**: Establishes address of recipient, repeated per recipient
- **DATA**: Signifies start of message text with header and body

| SMTP Code | Meaning                        |
| --------- | ------------------------------ |
| 220       | SMTP Service Ready             |
| 250       | Requested Action Completed     |
| 421       | Service Unavailable            |
| 450       | User's Mailbox Unavailable     |
| 451       | Recipient's Server Error       |
| 452       | Server Storage Insufficient    |
| 500       | Command Syntax Error           |
| 501       | Command Arguments Syntax Error |
| 503       | Bad Sequence of Commands       |
| 550       | User's Mailbox Unabailable     |
| 551       | Recipient Not Local            |
| 552       | Recipient's Email Full         |
| 554       | Delivery Error                 |
