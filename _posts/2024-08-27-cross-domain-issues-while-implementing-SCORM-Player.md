---
layout: post
title: Cross-domain issues while implementing SCORM Player
---
It wouldn’t be right to finish without mentioning cross-domain issues and SCORM. SCORMs typically track using a JavaScript API object exposed by an LMS. The LMS is required to call this object “API” and it must reside on the window of the LMS launching the SCORM.

The fun really starts if the LMS is on one domain and the SCORM that’s being launched is on another. Your LMS may be hosted on mylms.somewhere.com and your course hosted on mycourse.overthere.com. By definition, JavaScript can’t communicate easily across domains. While it’s possible with the help of some JavaScript trickery, most authoring tools don’t provide SCORMs that are cross-domain capable.

Once again, it’s important to ask an LMS provider if they’ve gone the extra mile to support cross-domain tracking with SCORM. It’s particularly important if your SCORMs are media-rich and require a Content Delivery Network (CDN, such as CloudFront) to deploy courses. At LearnUpon, we’ve taken that approach; it delivers a better experience to learners viewing courses that contain rich-media content delivered via the server closest to them. This is much better than relying on the server that hosts your LMS.

Hopefully, you now understand what the SCORM API is, and how it works. SCORM is just one of many eLearning content formats, with newer formats like xAPI (Tin Can) and cmi5 continuing to be developed. If you have any questions on the SCORM API, share your thoughts in the comments below.
