# Uncommon HTML Bug: Broken Image in innerHTML

This repository demonstrates a subtle HTML bug related to using innerHTML to inject content containing a broken image reference. The bug doesn't cause a JavaScript error, but it results in a broken image and might affect the overall layout of the page, leading to a degraded user experience.  The solution focuses on robust error handling and ensuring the image's availability before inclusion.

## Bug Description
The provided HTML code uses innerHTML to inject HTML content, including an image.  The image source (`broken-image.jpg`) is intentionally incorrect to trigger the bug. The bug's impact is primarily visual - a broken image icon replaces the expected image, potentially disrupting page layout.  The lack of explicit error handling makes this bug difficult to detect without visual inspection.

## Solution
The solution involves verifying the image's existence before injection, gracefully handling cases where the image is not found. This ensures a more robust and user-friendly experience.