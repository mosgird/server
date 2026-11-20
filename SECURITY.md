# Security policy

This repository holds the Mosgird relay server. The relay stores and forwards ciphertext and public keys. It is not meant to read message content. Problems here are high priority when they let the relay read plaintext, forge or swap public keys, or expose more metadata than the protocol describes.

## Reporting a vulnerability

Do not report security problems in a public issue or pull request.

Report them privately with GitHub's private vulnerability reporting: open the **Security** tab of this repository and choose **Report a vulnerability**. You can also go directly to https://github.com/mosgird/server/security/advisories/new.

Include:

- what the problem is, and where it is (file, endpoint, or commit);
- what an attacker could do with it, including whether message content, keys, identities, or metadata are exposed;
- steps to reproduce, or a proof of concept if you have one;
- whether you want to be credited.

We read every report. We do not yet guarantee a response time, and this page will say so if that changes.

## Scope

In scope: anything in this server that lets it or an outside party read message content, substitute public keys, forge identities, or learn metadata the protocol says is hidden. The protocol's requirements are in [mosgird/protocols](https://github.com/mosgird/protocols); a server that breaks them is in scope even when the protocol document itself is correct.

Out of scope: problems in third-party libraries, unless our use of them is at fault; reports that need access to systems you do not own; denial-of-service testing against infrastructure you do not own.

## Disclosure

We ask for coordinated disclosure: report first, give us a reasonable time to fix the problem, and do not publish details until a fix is released or we agree on a date. We credit reporters who want credit.

## Supported versions

No version is released yet. Only `main` is supported. When releases exist, this section lists which ones receive security fixes.
