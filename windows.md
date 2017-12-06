control /name Microsoft.DefaultPrograms

explorer.exe shell:recyclebinfolder

getmac

netstat /displaydns

mctadmin.exe - local package; mistni nastaveni; jazyk apod.

sfc.exe - system file checker

sysedit.exe  

netsh.exe

openfiles.exe (via cmd interpreter)

net config

ipconfig

wf.msc (windows firewall)

gpedit.msc (group policy editor)

secpol.msc (security policy editor)

mmc.exe (snap-in console)

route print

mrt.exe

systeminfo

regedit

gpupdate

gpresult

nslookup

pathping

tracert

mstsc /admin

fsutil

powercfg -h off (vypne podporu hibernace)

bootcfg

bootsect

bcdedit

doskey

gpresult /r

tasklist

time /t

chkdsk

recover

nltest (shutdowns, stoping process and many more..)

msiexec

wmic

winchat

diskpart

winrs

winrm

wbadmin

schtasks

cacls

runas

net use

subst

compmgmt.msc /s

diskmgmt.msc

dfrg.msc

services.msc /s

eventvwr.msc /s

devmgmt.msc

%SystemRoot%\system32\Com\comexp.msc

perfmon.msc /s

secpol.msc /s

lusrmgr.msc /s

***

Win7Config.{ED7BA470-8E54-465E-825C-99712043E01C}

***

__Custom logon text__

HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
	legalnoticecaption (RG_SZ)
	legalnoticetext (RG_SZ)

***

__Custom folder icon__

[.ShellClassInfo]
IconResource=C:\Windows\system32\SHELL32.dll,20

and/or

[.ShellClassInfo]
IconFile=%SystemRoot%\system32\SHELL32.dll
IconIndex=20

***

__Custom theme location__

C:\Users\jurcapavel\AppData\Roaming\Microsoft\Windows\ThemesComputer

***

__Netdiag Client Connectivity__

Ndis - Netcard queries test

IpConfig - IP config test

Member - Domain membership test

NetBT Transports - NetBT transports test

Autonet - Automatic Private IP Addressing (APIPA) address test

IpLoopBk - IP loopback ping test

DefGw - Default gateway test

NbtNm - NetBT name test

WINS - WINS service test

Winsock - Winsock test

DNS - DNS test

Browser - Redir and Browser test

DsGetDc - DC discovery test

DcList - DC list test

Trust - Trust relationship test

Kerberos - Kerberos test

Ldap - LDAP test

Route - Routing table test

Netstat - Netstat information test

Bindings - Bindings test

WAN - WAN configuration test

Modem - Modem diagnostics test

NetWare - NetWare test

IPX - IPX test

