-- --

This is Corban Pendrak's vault for cybersecurity resources and notes.

# Modules
- [[Hardware MOC]]
- [[Linux MOC]]
- [[Network MOC]]
- [[Offensive Security Concepts MOC]]
- [[Programming MOC]]
- [[Regular Expressions]]
- [[HackTheBox Writeups]]


> [!warning]- Fix backlinks (for Obsidian editing)
> ```base
> formulas:
> Backlinks: file.backlinks.filter(! file.hasLink(value)).map(value.asFile())
> Num Backlinks: file.backlinks.filter(! file.hasLink(value)).length
>views:
>  - type: table
>    name: Non-reciprocal Backlinks
>    filters:
>      and:
>        - file.name.contains("MOC")
>        - file.backlinks.length > 0
>        - file.backlinks.filter(! file.hasLink(value.asFile())).length > 0
>    order:
>      - file.name
>      - formula.Backlinks
>    sort:
>      - property: formula.Num Backlinks
>        direction: DESC
>    columnSize:
>      file.name: 213
>```
> file.backlinks.filter(! file.hasLink(value)).map(file)
# Todo
- research syscall hooking
- research linux kernel for persistence
	- dmesg is kernel log
- research rootkits
- char device interacts with kernel for privelige escalation
	- requires root, but useful for persistence, unless kernel bug
- Hooks replace kernel commands with user defined command
	- More hooks is more functionality.
	- tcp_seq_show hook for hiding from netstat
- Hide PID in /proc
- Don't dereference user memory in root/kernel
- Hide process in Windows in kernel \_EPROCESS double linked list
- Minifilters with highest altitude value allows for WIndows file hiding

```base
formulas:
  Backlinks: file.backlinks.filter(! file.hasLink(value)).map(value.asFile())
  Num Backlinks: file.backlinks.filter(! file.hasLink(value)).length
views:
  - type: table
    name: Table
    filters:
      and:
        - file.name.contains("MOC")
        - file.backlinks.length > 0
        - file.backlinks.filter(! file.hasLink(value.asFile())).length > 0
    order:
      - file.name
      - formula.Backlinks
    sort:
      - property: formula.Num Backlinks
        direction: DESC

```
