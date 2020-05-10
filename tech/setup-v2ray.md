---
layout: page
title: How to setup your v2ray?
subtitle: a powerful technique against IP banning
---

It is really an useful skill for people who live in China to setup a VPN. Considering the frequently ban of VPS on some protocols like Shadowsocks, I use the V2Ray. It has three disadvantages:
- **Security**: v2ray is a much more secure protocol than others.
- **Convenience**: there are many convenient scripts to configure v2ray
- **Effectiveness**: it cannot be banned when you use both v2ray and cdn. Otherwise, most other protocols can be banned and you need to find another one. It just wastes your money.

Welcome to the v2ray world!

- Target: setup a VPN for your own use.
- Cost: about $47 (330 RMB) per year and a bit of your rest time.
- Level: ⭐⭐⭐⭐

### 1. Buy a VPS

I choose the [![](https://bwh88.net/templates/organicbandwagon/images/logo.png)](https://bwh88.net/) for the reason in **price** and **convenience** (support for Alipay), however, there are some other kinds of VPS server providers with appealling prices, such as 

| :------ |:--- | :--- |
| Vultr | [https://www.vultr.com/](https://www.vultr.com/)| I tried|
| Linode | [https://www.linode.com/](https://www.linode.com/)| |

**Remember to use promotion code in BandwagonHOST!** It usually has a 6% discounting!

### 2. Powerful techniques (all are free!)
Against the banning of servers' IP in China, we choose another powerful technique to build our VPN server, rather the directly connecting by Shadowsocks protocol.

#### Register your free domain
I strongly recommend you to register a free domain in [![](https://my.freenom.com/templates/freenom/img/logo.png)](https://my.freenom.com/) because of its 12-month free domain service. However, you can register a new one when the date is out for our use. By the way, it is also okay to buy a domain in any other ways.

**Note:** You should create an account [here](http://www.freenom.com/en/developers.html).

#### Setup CDN for your domain

After registering the domain, we need to connect it with our VPS, i.e., the CDN service. Luckily, we can use the free service provided by [cloudflare.com](https://dash.cloudflare.com/). In its DNS dashboard, you shoud setup like following:

![](setup-v2ray-img-1.PNG)

**Note:** You should gray the status button. It may take a long time, and you need to continue the next step after days.

#### Install V2ray service in your VPS

We need to install v2ray service in our VPS by following command:

```bash
bash <(curl –s –L https://git.io/v2ray.sh)
```

and then install step by step (this script may be unavaible, please find another one in [Github](https://github.com) if it happens).