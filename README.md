# stUpiidhax: Wii U 5.5.2 browser pwn

This is the git repository for stUpiidhax, a very popular homebrew 
entrypoint access gate for the Wii U's 5.5.2 firmware.

- Hosted access gate urls:
- http://sleepii.ovh/
- http://stupiid.ovh/
- http://u.drg.li/

## JSTypeHax

This is based on the JumpCallPop JSTypeHax (aka WiiUTest) exploit. 

## The cg Method

The so-called `cg` method was used to improve reliability with some 
older versions of the exploit. I no longer believe that this is 
nesessary as the current `stable` exploit is quite reliable, but I 
figure it's worth documenting anyway.

With an old version of the exploit, it seemed more effective than 
placebo to run the access gate behind a very specific server 
configuration. We accidentally discovered that it seemed to help if the 
access gate was specifically hosted on GitHub Pages, but proxied 
behind Cloudflare's POPs. We tried Cloudflare's POPs in front of a 
normal server as well as GitHub Pages without Cloudflare's POPs, all 
to no avail. It seems something specific about running the gate on 
GitHub Pages and putting Cloudflare's DDOS protection service in front 
of it would cause the exploit to become more reliable.

Once again, I no longer believe this is nessesary or even useful with 
the current `stable` version, but I still believe that it's worth 
noting.

The cg method was accidentally discovered by 
me, and researched extensively by [ColtonDRG](https://twitter.com/coltondrg).

## And Finally, Credits

Once again, all credit for the exploit itself goes to JumpCallPop and 
everyone else who helped him get this working. I just made a nice gateway, 
helped lots of people get it working, and compiled all this information.

- [Original GBAtemp thread](https://gbatemp.net/threads/webhack-on-5-5-2-jstypehax.480938/)

- [coltondrg? Twitter](https://twitter.com/coltondrg)

- [Creatable Twitter](https://twitter.com/Creatable)

- [Colton's Repo (the one I ripped this from!)](https://git.coltondrg.com/stUpiidhax)