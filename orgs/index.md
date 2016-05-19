---
layout: page
title: Organizations
---

The organizations listed here fall under one of two tax codes, 501(c)(3) or
501(c)(6).

## 501(c)(3)

This is the most common type of nonprofit. It includes organizations that are
religious, educational, charitable, scientific, and literary; groups that test
for public safety, that foster national or international amateur sports competition;
or organizations engaged in the prevention of cruelty to children or animals.

This type of nonprofit applies for its status using IRS form 1023, and files
annually form 990, 990EZ, or 990-PF. Contributions are usually tax-exempt.

## 501(c)(6)

These organizations are business leagues, chambers of commerce, real estate
boards, etc. **They seek to improve business conditions.** They apply using IRS
form 1024 and file annually the 990 or 990EZ.

See [How the IRS Classifies Nonprofit Organizations](http://nonprofit.about.com/od/becomingtaxexempt/a/nonprofittypes.htm)
on About.com for more information.

## Organization Profiles

{% assign orgs = site.data.organizations | sort: name %}

{% for orghash in orgs %}
    {% assign orgkey = orghash[0] %}
    {% assign org = orghash[1] %}
* [{{ org.name }}](./{{ orgkey }})
{% endfor %}


