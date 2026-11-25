<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://sebsoft.nl/assets/sebsoft-logo-white.png">
  <img src="https://sebsoft.nl/assets/sebsoft-logo.png" alt="Sebsoft" height="52">
</picture>

### Open source Moodle plugins, kept working across versions

We are a Dutch development shop that has been building on Moodle since 2004.<br>
Everything published here is GPL-3.0-or-later. Nearly all of it is free to use, with or without us;
where a subscription applies, the table says so.

![Moodle 4.2 to 5.3](https://img.shields.io/badge/Moodle-4.2%20to%205.3-F98012?style=flat-square&logo=moodle&logoColor=white)
[![19 plugins on the Moodle Marketplace](https://img.shields.io/badge/Moodle%20Marketplace-19%20plugins-0c1e32?style=flat-square)](https://marketplace.moodle.com/user/827)
![GPL-3.0-or-later](https://img.shields.io/badge/licence-GPL--3.0--or--later-1647ff?style=flat-square)
[![Sponsor](https://img.shields.io/badge/sponsor-%E2%99%A5-db61a2?style=flat-square)](https://github.com/sponsors/sebsoftnl)
[![sebsoft.nl](https://img.shields.io/badge/sebsoft.nl-%E2%86%97-14784b?style=flat-square)](https://sebsoft.nl)

</div>

---

Most of what we publish started as a client problem that Moodle core does not solve: a customer
wanted to hand out access codes, take payments without bolting a webshop onto their LMS, or stop
their user list from filling up with people who left years ago. We built it once, released it, and
have been keeping it alive through every Moodle version since. The oldest of them has been in the
public plugin directory since 2015.

This organisation is our open source shelf, and it is a mirror: the development itself happens on
our own GitLab and is pushed here. It is not the whole of what we build, and the plugins below are
the part we publish.

Each plugin links to its repository. The Moodle column is the version range of the latest release,
and the last column is where to get it: the [Moodle Marketplace](https://marketplace.moodle.com/user/827),
and [CAMP](https://camp-registry.org/), the independent Community Archive of Moodle Plugins, which
rebuilds a package from the maintainer's tagged release and hash-compares it before it carries a
badge.

## 🎟️ Coupon suite

Someone gets a code and lands in the right course, without you creating an enrolment by hand for
every participant.

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`block_coupon`](https://github.com/sebsoftnl/moodle-block_coupon) | Generates coupon codes for courses, groups or cohorts and sends them by email or as a PDF | 4.5 to 5.2 | [Marketplace](https://marketplace.moodle.com/plugins/block_coupon) · [CAMP](https://camp-registry.org/plugin/block_coupon.html) |
| [`auth_coupon`](https://github.com/sebsoftnl/moodle-auth_coupon) | Lets someone in with just a coupon code and email address; the account is created along the way | 4.2 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/auth_coupon) · [CAMP](https://camp-registry.org/plugin/auth_coupon.html) |
| [`profilefield_coupon`](https://github.com/sebsoftnl/moodle-profilefield_coupon) | Processes a coupon code entered in a profile field during registration | 4.5 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/profilefield_coupon) · [CAMP](https://camp-registry.org/plugin/profilefield_coupon.html) |
| [`filter_couponinput`](https://github.com/sebsoftnl/moodle-filter_couponinput) | Places a coupon input field anywhere Moodle filters are applied *(alpha)* | 4.5 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/filter_couponinput) · [CAMP](https://camp-registry.org/plugin/filter_couponinput.html) |

> The suite handles access, not payment. If someone should pay first, combine it with the payment
> plugins below.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-coupon-plugins](https://sebsoft.nl/en/moodle-coupon-plugins/)</sub>

## 💳 Payments

Moodle has had its own payment gateway system since 4.0. These plugins cover the practical side on
top of it, plus the Dutch providers core does not ship.

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`enrol_gwpayments`](https://github.com/sebsoftnl/moodle-enrol_gwpayments) | Paid enrolment on a course, with discount coupons that have a validity period and a usage cap | 4.4 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/enrol_gwpayments) · [CAMP](https://camp-registry.org/plugin/enrol_gwpayments.html) |
| [`mod_gwpayments`](https://github.com/sebsoftnl/moodle-mod_gwpayments) | A payment as a standalone activity, for example for exam fees or materials | 4.2 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/mod_gwpayments) · [CAMP](https://camp-registry.org/plugin/mod_gwpayments.html) |
| [`availability_gwpayments`](https://github.com/sebsoftnl/moodle-availability_gwpayments) | Makes access to a section or activity conditional on a completed payment | 4.2 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/availability_gwpayments) · [CAMP](https://camp-registry.org/plugin/availability_gwpayments.html) |
| [`report_gwpayments`](https://github.com/sebsoftnl/moodle-report_gwpayments) | Reporting on the payments made through the Gateway Payments plugins | see repo | [CAMP](https://camp-registry.org/plugin/report_gwpayments.html) |
| [`paygw_mollie`](https://github.com/sebsoftnl/moodle-paygw_mollie) | Payment gateway for Mollie, covering iDEAL, credit card and Bancontact among others | 4.4 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/paygw_mollie) · [CAMP](https://camp-registry.org/plugin/paygw_mollie.html) |
| [`paygw_paynl`](https://github.com/sebsoftnl/moodle-paygw_paynl) | Payment gateway for PAY. (Pay.nl) | 3.10 to 3.11 | [Marketplace](https://marketplace.moodle.com/plugins/paygw_paynl) · [CAMP](https://camp-registry.org/plugin/paygw_paynl.html) |
| [`enrol_classicpay`](https://github.com/sebsoftnl/moodle-enrol_classicpay) | The predecessor of Gateway Payments, from before payments existed in core. Maintained for existing installations | 4.0 to 4.5 | [Marketplace](https://marketplace.moodle.com/plugins/enrol_classicpay) · [CAMP](https://camp-registry.org/plugin/enrol_classicpay.html) |

> We are not a payment service provider. The contract and the money run directly between you and
> Mollie or PAY.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-payment-plugins](https://sebsoft.nl/en/moodle-payment-plugins/)</sub>

## 👥 User lifecycle

Moodle creates accounts easily and rarely cleans them up. These two automate the cleanup, and make
it reversible.

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`tool_usersuspension`](https://github.com/sebsoftnl/moodle-tool_usersuspension) | Suspends accounts automatically and deletes them afterwards according to your rules, with exclusion lists for accounts that must always stay | 4.4 to 5.0 | [Marketplace](https://marketplace.moodle.com/plugins/tool_usersuspension) · [CAMP](https://camp-registry.org/plugin/tool_usersuspension.html) |
| [`tool_userrestore`](https://github.com/sebsoftnl/moodle-tool_userrestore) | Restores accounts Moodle has deleted, including the enrolments and results attached to them | 4.2 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/tool_userrestore) · [CAMP](https://camp-registry.org/plugin/tool_userrestore.html) |

> Cleanup runs on Moodle cron. If your cron is unreliable, nothing happens. That is the most common
> cause of "the plugin does nothing".

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-user-lifecycle-plugins](https://sebsoft.nl/en/moodle-user-lifecycle-plugins/)</sub>

## 🔒 Security

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`auth_antihammer`](https://github.com/sebsoftnl/moodle-auth_antihammer) | Detects repeated login attempts and blocks by IP address, by username or by both. You define what counts as "too many" | 3.10 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/auth_antihammer) · [CAMP](https://camp-registry.org/plugin/auth_antihammer.html) |

> This protects the Moodle login screen, not your whole server, and it does not replace two-factor
> authentication. It limits how often someone may try.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-security-plugins](https://sebsoft.nl/en/moodle-security-plugins/)</sub>

## 📱 SMS gateways

Moodle 4.5 introduced an SMS subsystem but ships almost no providers. We built four. Technically
they are interchangeable, so pick on price, coverage, or the contract you already have.

| Plugin | Why you would pick this one | Moodle | Install from |
| --- | --- | --- | --- |
| [`smsgateway_textmagic`](https://github.com/sebsoftnl/moodle-smsgateway_textmagic) | Fastest to set up: create an account, paste the API key, done. No separate sender registration to get going | 4.5 to 5.0 | [Marketplace](https://marketplace.moodle.com/plugins/smsgateway_textmagic) · [CAMP](https://camp-registry.org/plugin/smsgateway_textmagic.html) |
| [`smsgateway_sinch`](https://github.com/sebsoftnl/moodle-smsgateway_sinch) | The heaviest of the four in reach and delivery guarantees. The choice for international sending or verifiable delivery reporting | 4.5 to 5.0 | [Marketplace](https://marketplace.moodle.com/plugins/smsgateway_sinch) · [CAMP](https://camp-registry.org/plugin/smsgateway_sinch.html) |
| [`smsgateway_messagebird`](https://github.com/sebsoftnl/moodle-smsgateway_messagebird) | A Dutch provider, which keeps the processing-agreement discussion inside the EU | 4.5 to 5.0 | [Marketplace](https://marketplace.moodle.com/plugins/smsgateway_messagebird) · [CAMP](https://camp-registry.org/plugin/smsgateway_messagebird.html) |
| [`smsgateway_plivo`](https://github.com/sebsoftnl/moodle-smsgateway_plivo) | Per-message pricing without a subscription, which suits low or irregular volumes such as two-factor at login only | 4.5 to 5.0 | [Marketplace](https://marketplace.moodle.com/plugins/smsgateway_plivo) · [CAMP](https://camp-registry.org/plugin/smsgateway_plivo.html) |

> Requires Moodle 4.5 or later, plus an account and API key with the provider. You pay the provider
> for the messages; we only supply the integration.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-sms-plugins](https://sebsoft.nl/en/moodle-sms-plugins/)</sub>

## 📣 Announcements

Notices that appear and disappear on their own, so nobody has to remember to take them down after
the maintenance window closes.

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`local_plannot`](https://github.com/sebsoftnl/moodle-local_plannot) | Schedules a message with a start and end date, site-wide or inside a single course, with a choice of audience, placement, styling and how it can be dismissed *(paid)* | 4.5 to 5.2 | [Marketplace](https://marketplace.moodle.com/plugins/local_plannot) |

> This one runs on a paid subscription, unlike everything else on this page. The code is still
> GPL-3.0-or-later and ships inside the plugin; what the subscription pays for is the releases, the
> updates and the support. The repository linked above is an issue tracker and holds no source.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-announcement-plugins](https://sebsoft.nl/en/moodle-announcement-plugins/)</sub>

## 🤖 AI assistants for teachers

A teacher connects Claude, ChatGPT or another MCP client to Moodle and gets help with their own
courses, limited to what Moodle already allows them to do.

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`tool_teachermcp`](https://github.com/sebsoftnl/moodle-tool_teachermcp) | Gives a teacher's AI assistant an authenticated MCP endpoint to read course materials, create pages, quizzes and H5P activities, and prepare grading *(beta)* | 4.5 to 5.3 | [CAMP](https://camp-registry.org/plugin/tool_teachermcp.html) |

> Course materials and student data, hidden ones included, can be sent to the AI service you
> connect. Use test data until your organisation has agreed what may be shared. The AI client and
> any subscription it needs are separate from the plugin.

<sub>Installation and client setup: [the repository README](https://github.com/sebsoftnl/moodle-tool_teachermcp#readme)</sub>

## 🔤 Fonts and PDF

| Plugin | What it does | Moodle | Install from |
| --- | --- | --- | --- |
| [`tool_tcpdffonts`](https://github.com/sebsoftnl/moodle-tool_tcpdffonts) | Converts and manages your own fonts for Moodle's PDF output from the admin interface, and stores them outside core so an upgrade does not wipe them | 4.2 to 5.1 | [Marketplace](https://marketplace.moodle.com/plugins/tool_tcpdffonts) · [CAMP](https://camp-registry.org/plugin/tool_tcpdffonts.html) |
| [`tiny_fonttools`](https://github.com/sebsoftnl/moodle-tiny_fonttools) | Extends the font choices in the TinyMCE editor, so what an author picks matches what comes out in the PDF *(in development)* | see repo | [CAMP](https://camp-registry.org/plugin/tiny_fonttools.html) |

> Adding a font does not mean you may use it: check whether the licence permits embedding in a PDF.

<sub>Use cases, limitations and FAQ: [sebsoft.nl/en/moodle-font-plugins](https://sebsoft.nl/en/moodle-font-plugins/)</sub>

## How we maintain this

- **These repositories mirror our own GitLab.** Development happens there and is pushed here, so
  history can arrive in larger steps than one commit at a time.
- **Bugs and pull requests are welcome here on GitHub.** Open an issue on the repository in
  question and include your Moodle version, the plugin version and what you expected to happen. We
  read them here; a change we accept travels through our GitLab and returns on the next push.
- **Version support follows our clients.** When a Moodle release lands, we test and bump the
  plugins that run in production somewhere, and drop support for versions that are out of Moodle's
  own support window.
- **Not everything we build is distributed through a registry**, so if a plugin is missing from
  both the Marketplace and CAMP, ask rather than assume it is gone.
- **Security issues:** please report those privately to
  [helpdesk@sebsoft.nl](mailto:helpdesk@sebsoft.nl) rather than in a public issue.

## Supporting this work

Nearly all of these plugins are free. Keeping them working across every Moodle release is not, and
that part is paid for out of client work. If your organisation runs on them, there are three ways
to help carry it:

- **[Sponsor us on GitHub](https://github.com/sponsors/sebsoftnl)** for a recurring amount, which is
  what makes maintenance predictable rather than something we fit in between projects.
- **[Make a one-off contribution](https://customerpanel.sebsoft.nl/sebsoft/donate/intro.php)** if a
  specific plugin saved you a job you were dreading.
- **[Ask about a support contract](https://sebsoft.nl/en/contact/?over=plugin-support#aanvraag).** Free
  plugins come with community support. A contract buys a guaranteed response time, urgent fixes and
  changes built for your situation. The form opens with the question already filled in, so it takes
  a minute.

Contributing a patch, a translation or a well-written bug report is worth just as much, and costs
nothing.

## Beyond what is published here

Open source is a deliberate part of what we do, not all of it. Scheduled Messages above is sold
rather than given away, and there is more of that kind: plugins we license commercially, and work
written for one organisation that stays with that organisation. Most of it never reaches a public
registry, so a plugin you cannot find here may still exist.

The rest of our work sits in the same place: [custom Moodle
development](https://sebsoft.nl/en/moodle-plugin-development/), integrations with the systems you
already run, technical audits, and hosting for [Moodle](https://sebsoft.nl/en/moodle-hosting/) and
[BigBlueButton](https://sebsoft.nl/en/bigbluebutton/). If you are weighing up whether something is
worth building, a technical conversation costs nothing.

<div align="center">

**[sebsoft.nl](https://sebsoft.nl)** &nbsp;·&nbsp;
[Plugin overview](https://sebsoft.nl/en/plugins/) &nbsp;·&nbsp;
[Book a technical call](https://meet.sebsoft.nl/sebastian/technisch-adviesgesprek-moodle?lang=en) &nbsp;·&nbsp;
[helpdesk@sebsoft.nl](mailto:helpdesk@sebsoft.nl)

<sub>Sebsoft B.V. · Vang 14a, 4661 TX Halsteren, the Netherlands · Chamber of Commerce 64822028</sub>

</div>
