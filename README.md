# Kernel-s-Homebrew
Kernel's(public) homebrew

------ PS4 Update Blocker ------

UP7985-CUSA79863_00-E0TG962ITXST0L6L-A0100-V0100.pkg ; PS4 Update Blocker Remover ; MD5:798b128c353b2237df4b43215ae2488c

UP5678-CUSA56793_00-SIYVA5IIZT7JCWAG-A0100-V0100.pkg ; PS4 Update Blocker Installer ; MD5:e05294e8a464131772e12ad30a06ec01

UP4102-CUSA41028_00-UIGM2D10K9JMCG25-A0100-V0100.pkg ; PS4 Update Blocker Remover 6.72 ; MD5:0e7dcf287c3a5f38d5d315e82c8c6032

UP7841-CUSA78420_00-DFWM2CXWDPK0ED9Q-A0100-V0100.pkg ; PS4 Update Blocker Installer 6.72 ; MD5:a90c23943496a87d5f70e8046761d076

ONLY INSTALL THE ONE FOR YOUR SYSTEM VERSION

=======Installation========

*1: Put on a USB install via debug settings OR use Remote PKG Installer

*2: profit!?!?!

=======Compatabilty=======

for the time being, 5.05 and 6.72 only;

=======Usage=======

you want to remove the update blocker?, open the remover;

you want to install the update blocker?, open the installer

=======How It Works=======

updates and thier temp download spot is /update and thier name usally is "PS4UPDATE.PUP" for downloaded updates and "PS4UPDATE.PUP.net.temp" for downloading ones, you could remove them via FTP if needed, but who wants to even let it download them? nobody
so what this does is it creates an FOLDER with the same name so when the system try's to delete the old one and download the update it can't so it will fail, how does this app do it?, it breakes outside of the sandbox and calls sceKernelUnlink() than calls sceKernelMkdir()
once it does that it calls std::cin.get(); to pervent the app from returning so it does not crash.

=======Notes=======

It uses Retail offsets so it will only work on Retail(maybe testkit though im not sure)

If a update files does exists, you need to remove it, either by FTP or by deleteing it in the playstation menu.

It does take a few seconds to do the porcess so give it 5 ish seconds and than you can close the app.

it does boot to a black-screen and there is no user input or menues, so keep that in mind.

This was not made in unity.

=======Credits=======

Thanks:
- [zecoxao](https://github.com/zecoxao) - For his fork of PS4_UnjailPlugin_Unity_NativeCode
- [SocraticBliss](https://github.com/SocraticBliss)
- samsepi
- [Lapy](https://github.com/Lapy055)
- [AlAzif](https://github.com/Al-Azif)
- [AlberzH0fi](https://twitter.com/lukas_pedall) - for testing my 6.72 version
