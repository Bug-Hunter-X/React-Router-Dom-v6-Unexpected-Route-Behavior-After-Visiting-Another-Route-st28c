# React Router Dom v6 Unexpected Route Behavior

This repository demonstrates a bug in React Router Dom v6 where unexpected route behavior occurs when navigating to a specific path after visiting another path. The issue only seems to appear after interacting with another route like '/about'.

## Bug Description

The bug is reproducible in a simple app using React Router Dom v6. Navigating to '/contact' directly works fine.  However, if you first navigate to '/about' and *then* try to go to '/contact', the application will unexpectedly not render the component for the '/contact' path.  It might show a blank screen or a fallback UI.

## Solution

The solution involves ensuring that the path for your routes are correctly defined and don't have any conflicts.  Double-check for typos, and verify that the components being associated with the routes are correctly exported and imported.