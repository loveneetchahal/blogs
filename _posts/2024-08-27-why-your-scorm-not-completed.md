---
layout: post
title: Why did your SCORM content not get completed?
---
If your SCORM content cannot be completed, there are two possible reasons:

The completion rules are not properly set during production.
The completion rules must be set within the tool to create the SCORM file. To ensure your SCORM content works properly, you can always test it in SCORM Cloud.

SCORM content that’s embedded in iFrames doesn’t auto-refresh when completed.
Your SCORM content might be designed to be executed inside a pop-up window and send the data after the window closes. When embedded, the SCORM content doesn't send any data before being unloaded, and there’s no way around this restriction. You can verify whether or not that’s the case with your authoring tool's support service.
