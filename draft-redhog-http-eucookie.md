---
###
# Internet-Draft Markdown Template
#
# Rename this file from draft-todo-yourname-protocol.md to get started.
# Draft name format is "draft-<yourname>-<workgroup>-<name>.md".
#
# For initial setup, you only need to edit the first block of fields.
# Only "title" needs to be changed; delete "abbrev" if your title is short.
# Any other content can be edited, but be careful not to introduce errors.
# Some fields will be set automatically during setup if they are unchanged.
#
# Don't include "-00" or "-latest" in the filename.
# Labels in the form draft-<yourname>-<workgroup>-<name>-latest are used by
# the tools to refer to the current version; see "docname" for example.
#
# This template uses kramdown-rfc: https://github.com/cabo/kramdown-rfc
# You can replace the entire file if you prefer a different format.
# Change the file extension to match the format (.xml for XML, etc...)
#
###
title: "HTTP extension for the EU cookie law"
abbrev: "EUCOOKIE"
category: info

docname: draft-redhog-http-eucookie-latest
submissiontype: independent  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: AREA
workgroup: WG Working Group
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: WG
  type: Working Group
  mail: WG@example.com
  arch: https://example.com/WG
  github: USER/REPO
  latest: https://example.com/LATEST

author:
 -
    fullname: Egil Moeller
    organization: RedHog
    email: redhog@redhog.org

normative:

informative:


--- abstract

This document defines a HTTP protocol extension to handle cookie options to fullfill the cookie provisions of the EU GDPR (the cookie law) while avoiding superflous cookie popups and allowing users to set general policy on cookies.

--- middle

# Introduction

## Purpose

## Implementation

This document defines a new [HTTP response header](https://www.rfc-editor.org/rfc/rfc2616#section-6.2) `cookie-classes` and a new [HTTP request header](https://www.rfc-editor.org/rfc/rfc2616#section-5.3) `cookie-policy` that can be used by the client to query the server about what classes of cookies it would like to set, and to inform the server what classes of cookies are in fact acceptable to set.

These headers are acceptable for all HTTP methods. In particular, the OPTIONS method could be used by a client to acquire the `cookie-classes` header value wiuthout retreiving a full document.

### cookie-policy format

If present, the cookie policy header must conatain a list of cookie class names, separated by comma. Only cookies falling into one of the listed classes



TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
