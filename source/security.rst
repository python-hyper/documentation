Security
========

Our Goals
---------

When it comes to security issues, the Hyper project has one goal: to be
`tough and competent`_.

Security issues have real effects on real users, and it is the duty of library
authors to protect users from those problems as much as possible. As a result,
security is a paramount focus for our project, because if we fail and users are
exploited or made vulnerable, we are to blame.

This attitude leads to the following guidelines for contributors and
maintainers:

- The default configuration of a Hyper project **must** be as secure as
  possible.
- Any change that weakens the security of the default configuration of a Hyper
  project is to be resisted.
- We will react swiftly to being notified of security vulnerabilities.
- When notified of security vulnerabilities we will treat them all as serious
  incidents until otherwise determined: *there is no such thing as a
  severity security bug*.
- We will work with downstream maintainers to backport patches to all versions
  of the software that are affected by a vulnerability, regardless of whether
  that version is still actively supported by the core team.
- It is better to break functioning-but-insecure code than it is to leave
  unaware users vulnerable.
- If and when we break functioning-but-insecure code, we will provide error
  messages that adequately explain the problem.
- Any insecure or less secure options made available in a Hyper project must
  cause warnings to be issued when used.


Vulnerability Disclosure
------------------------

If you think you have found a potential security vulnerability in a Hyper
project, please email `Lukasa`_ directly. **Do not file a public issue.**

Lukasa's PGP Key fingerprint is:

    - 90DC AE40 FEA7 4B14 9B70 662D F25F 2144 EEC1 373D


If English is not your first language, please try to describe the problem and
its impact to the best of your ability. For greater detail, please use your
native language and we will try our best to translate it using online services.

Please also include the code you used to find the problem and the shortest
amount of code necessary to reproduce it.

Please do not disclose this to anyone else. We will retrieve a CVE identifier
if necessary and give you full credit under whatever name or alias you provide.
We will only request an identifier when we have a fix and can publish it in a
release.

We will respect your privacy and will only publicize your involvement if you
grant us permission.

Process
~~~~~~~

This following information discusses the process the Hyper project follows in
response to vulnerability disclosures. If you are disclosing a vulnerability,
this section of the documentation lets you know how we will respond to your
disclosure.

Timeline
^^^^^^^^

When you report an issue, one of the project members will respond to you within
two days at the outside. In most cases responses will be faster, usually within
12 hours. This initial response will at the very least confirm receipt of the
report.

If we were able to rapidly reproduce the issue, the initial response will also
contain confirmation of the issue. If we are not, we will often ask for more
information about the reproduction scenario.

Our goal is to have a fix for any vulnerability released within two weeks of
the initial disclosure. This may potentially involve shipping an interim
release that simply disables function while a more mature fix can be prepared,
but will in the vast majority of cases mean shipping a complete release as soon
as possible.

Throughout the fix process we will keep you up to speed with how the fix is
progressing. Once the fix is prepared, we will notify you that we believe we
have a fix. Often we will ask you to confirm the fix resolves the problem in
your environment, especially if we are not confident of our reproduction
scenario.

At this point, we will prepare for the release. We will obtain a CVE number if
one is required, providing you with full credit for the discovery. We will also
decide on a planned release date, and let you know when it is. This release
date will *always* be on a weekday.

At this point we will reach out to our major downstream packagers to notify
them of an impending security-related patch so they can make arrangements. In
addition, these packagers will be provided with the intended patch ahead of
time, to ensure that they are able to promptly release their downstream
packages. Currently the list of people we actively contact *ahead of a public
release* is empty. We will notify these individuals at least a week ahead of
our planned release date to ensure that they have sufficient time to prepare.
If you believe you should be on this list, please let one of the maintainers
know at one of the email addresses at the top of this article.

On release day, we will push the patch to our public repository, along with an
updated changelog that describes the issue and credits you. We will then issue
a PyPI release containing the patch.

At this point, we will publicise the release. This will involve mails to
mailing lists, Tweets, and all other communication mechanisms available to the
core team.

We will also explicitly mention which commits contain the fix to make it easier
for other distributors and users to easily patch their own versions of the
project if upgrading is not an option. We will also work with downstream
distributors to patch their software.
