---
layout: page
title: Security advisories
permalink: /security/
---

IdPy projects, particularly the IdPy libraries (pySAML2, pyXMLSecurity,
pyeleven, oidcendpoint, and JWT-Connect-Python), are used by services around
the world. IdPy has a [security incident handling process][idpy-incident-response]
that applies to all IdPy projects. Security vulnerabilities reported for an
IdPy project are handled as responsibly and publicly as possible, following
GitHub’s guidance on managing these types of vulnerabilities.


## FAQ

- Are CVEs created for each security vulnerability?

  Yes. Each vulnerability that is reported and verified is assigned a CVE
  identifier. This is part of the incident-response handling process that IdPy
  follows. Security advisories are managed through GitHub and use GitHub as the
  CVE Numbering Authority (CNA). Further information on how security advisories
  are managed through GitHub can be found at “[About GitHub’s Security
  Advisories][gh-sec-advisories]”.

- How is the community notified of vulnerabilities and associated patches?

  IdPy has multiple communication channels; the [IdPy mailing list][idpy-ml],
  the [IdPy slack workspace][idpy-slack] ([invitation][idpy-slack-invite]) and
  project-specific mailing lists.

  When a new vulnerability is reported and verified, a new security advisory is
  created on GitHub and the issue is assigned a CVE identifier. Progress on the
  mitigation is tracked on a private fork, where the incident-response team and
  developers communicate to fix the issue.

  When the fix is ready, a release plan is prepared and all communication
  channels are used to notify the community of the presence of a new issue and
  the expected release plan. This allows the community time to prepare for a
  security upgrade. (Notice that security fixes are not backported at the
  moment.)

  When the advisory is published, GitHub automatically notifies all associated
  projects of the published advisory. Projects that use IdPy projects as
  dependencies should automatically get Pull Requests by dependabot.
  Additionally, all communication channels are used again, to notify the
  community of the release of a new version of the affected software that
  contains the relevant fixes that mitigate the reported issue.

- Is there a mailing list I can join to receive security announcements?

  At this moment, there is no separate list with security announcements. We
  announce new and upcoming releases on the idpy-discuss mailing list and the
  relevant project lists. These lists have more traffic than just release or
  security announcements.

  As another option, one can subscribe to notifications about new releases
  using the “watch” mechanism provided by GitHub. When a new release is out, it
  is tagged and uploaded both on pypi and GitHub. You can find information
  about subscribing to releases on the GitHub documentation section
  “[Configuring your watch settings for an individual
  repository][gh-watch-individual]”.

- What is the best approach to mitigate an issue?

  Upgrade to the latest version. At this point, IdentityPython does not have
  the resources required to provide backports of security issues or other
  fixes. We urge the community to try to keep up with the latest version. The
  organization advocates FOSS and is open to new colaborators. Since,
  everything is open, users are free to backport patches on their own.


## List of published security advisories

- CVE-2021-21239 - PySAML2 - To be announced on 2021/01/20
- CVE-2021-21238 - PySAML2 - To be announced on 2021/01/20
- [CVE-2020-5390] - PySAML2 - Improper Verification of Cryptographic Signature


  [idpy-incident-response]: https://github.com/IdentityPython/Governance/blob/master/idpy-incidentresponse.md
  [idpy-ml]: https://lists.sunet.se/listinfo/idpy-discuss
  [idpy-slack]: https://identity-python.slack.com
  [idpy-slack-invite]: https://join.slack.com/t/identity-python/shared_invite/enQtNzEyNjU1NDI1MjUyLTM2MWI5ZGNhMTk1ZThiOTIxNWY2OTY1ODVmMWNjMzUzMTYxNTY5MzE5N2RlYjExZTIyM2MwYjBjZGE4MGVlMTM

  [gh-sec-advisories]: https://docs.github.com/en/github/managing-security-vulnerabilities/about-github-security-advisories
  [gh-watch-individual]: https://docs.github.com/en/github/managing-subscriptions-and-notifications-on-github/viewing-your-subscriptions#configuring-your-watch-settings-for-an-individual-repository

  [CVE-2020-5390]: https://github.com/advisories/GHSA-qf7v-8hj3-4xw7
