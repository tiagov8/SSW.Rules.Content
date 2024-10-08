---
seoDescription: Migrate VSS history to TFS when necessary, considering frequent check-ins, decommissioning old VSS, or active projects.
type: rule
archivedreason:
title: Do you need to migrate the history from VSS to TFS?
guid: c4f91635-787a-4d8e-b5be-ffa8f9125e7f
uri: do-you-need-to-migrate-the-history-from-vss-to-tfs
created: 2011-11-18T03:52:46.0000000Z
authors:
  - title: David Klein
    url: https://ssw.com.au/people/david-klein
    noimage: true
  - title: Justin King
    url: https://ssw.com.au/people/justin-king
  - title: Ryan Tee
    url: https://ssw.com.au/people/ryan-tee
    noimage: true
  - title: Tristan Kurniawan
    url: https://ssw.com.au/people/tristan-kurniawan
related: []
redirects: []
---

Normally, you don't need to check the history very often. If you do need sometimes, then get it from VSS - Save much space for TFS. For example, we have a about 7G VSS history database, and we may only need a small bit of them every 3 months, so what's the point of coping about 7G file when we only need one line of code?

<!--endintro-->

But there are also some considerations that you may want to migrate the history:

* If the history of source changes will be checked very often, so you can check the old history with the recent together via TFS
* You are going to decommission the old VSS completely. Say you don't want to keep the old VSS database, and then it will be necessary to keep the information somewhere
* If the project is very active, then it will be worthy to migrate the history because your developers may need them every day

If you are going to move the history, the links may help:

* [Walkthrough: Migrating from Visual SourceSafe to Team Foundation](https://learn.microsoft.com/en-us/previous-versions/visualstudio/visual-studio-2008/ms181247(v=vs.90)?redirectedfrom=MSDN)
* [Migrating from SourceSafe to Team Foundation Server](https://devblogs.microsoft.com/buckh/migrating-from-sourcesafe-to-team-foundation-server/)
