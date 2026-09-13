# Security Policy

This policy applies to every repository in this organisation that does not carry
a `SECURITY.md` of its own.

## Reporting a vulnerability

**Use the "Report a vulnerability" button on the Security tab of the repository
in question.** It opens a private advisory that only the maintainers can see, so
the issue stays confidential while it is being fixed.

A GitHub account is required for that form — creating one is free. If you cannot
or do not want to use GitHub, write to **security@edutap.eu**.

> **That address is a mailing list and is not encrypted.** Anything you send to
> it is readable by whoever operates the mail infrastructure along the way. Do
> not put exploit details, credentials or personal data in that mail. Use it to
> ask for another channel, and we will arrange one.

Please do not open a public issue for a suspected vulnerability. A public issue
is a disclosure, and it happens before anyone has had a chance to react.

## What is worth reporting — and what is already known

The container images published from these repositories are scanned for known
vulnerabilities **every day**, and the findings are public: they are on the
Security tab of each repository, under "Code scanning". Most of them come from
the Debian base image — `openssl`, `perl`, `libpcre2` and their relatives — and
they are there for everyone to read.

**Those findings do not need to be reported.** We already know, and the list is
open precisely so that nobody has to ask. If one of them matters more than the
report suggests — because of how *we* use the affected package — that is worth
telling us, and the reasoning is the valuable part.

What we do want to hear about:

- a flaw in our own code: authentication, authorisation, input handling, the
  handling of tokens and secrets
- a configuration in what we publish that is unsafe by default
- credentials, keys or tokens that we have accidentally committed
- a way to make one of our services do something it should not, for someone who
  should not be able to

## What happens next

We will confirm that your report arrived and tell you what we think of it. We do
this as quickly as we can manage.

**We do not promise a deadline.** eduTAP is open source, maintained by people
with other duties; a fixed response time would be a promise we could not keep
reliably, and a broken promise is worse than none. What we do commit to is that
a report will not be ignored, and that you will hear from us rather than be left
guessing.

## Supported versions

Only the current state of the default branch is supported, and for published
container images only the most recently built image.

There are no maintenance branches: a fix goes into the current development line
and is published from there. If you run an older build, the answer to a security
problem will be to move to the current one.

Repositories that publish a versioned library carry their own `SECURITY.md` with
a version table; this file does not override it.
