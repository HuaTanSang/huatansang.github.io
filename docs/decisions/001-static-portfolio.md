# Use plain HTML and CSS for the portfolio

Date: 2026-11-07
Status: accepted

## Context

The portfolio needs a minimal introduction, project list, and contact links.
There is no existing application stack or dynamic behavior to preserve.

## Decision

Use static HTML pages and a shared stylesheet, with system fonts and CSS media
queries for mobile layouts and automatic dark mode. Keep personal content in
the HTML. Directory index files provide routes such as `/cv/` without a router.

## Alternatives considered

A framework or static site generator would add dependencies and a build step
without improving this single-page site.

## Consequences

The site works on any static host that serves directory index files. Content
changes require editing HTML. Reconsider a static site generator if content pages make
shared layouts difficult to maintain. Publishing is outside this task.
