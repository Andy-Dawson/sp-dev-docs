---
title: Performance
ms.date: 04/21/2020
ms.localizationpriority: medium
---
# Performance

## Summary

Implementing customizations in SharePoint places an even greater emphasis on effective design and development for web applications in general, and client-side web applications in particular, especially when it comes to the concept of application performance. Performance is one of the important factors that influence user-experience and how efficient users can work with the portal.

## High-level guideline/general rules

- When testing performance, take into account both server-side performance of your code, as well as the performance of your code running in end-users' browsers.
- Whenever possible cache data to minimize the number of requests to SharePoint.
- When referencing scripts and other assets, allow users to cache them for as long as possible to minimize the number of requests to the server and the amount of data to load.
- Avoid excessive DOM manipulation that would trigger re-rendering of the page and delay its loading.

## Handling SharePoint Online throttling

_**Applies to:** Office 365_

SharePoint Online uses throttling to prevent users from over-consuming resources. When a user runs CSOM or REST code that exceeds usage limits, SharePoint Online throttles any further request from the user for a period of time.

### Articles

- [Handle SharePoint Online throttling by using exponential back off](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

### Samples

- [SharePoint Online Throttling](https://github.com/SharePoint/PnP/tree/master/Samples/Core.Throttling)

## SharePoint Framework

_**Applies to:** Office 365 | SharePoint Server_

### Articles

- [Optimize builds for production](https://docs.microsoft.com/sharepoint/dev/spfx/toolchain/optimize-builds-for-production)
- [JavaScript Patterns and Performance](https://docs.microsoft.com/sharepoint/dev/solution-guidance/javascript-patterns-and-performance)
- [Make batch requests with the REST APIs](https://docs.microsoft.com/sharepoint/dev/sp-add-ins/make-batch-requests-with-the-rest-apis)
- [SharePoint Framework (SPFx) enterprise guidance](https://docs.microsoft.com/sharepoint/dev/spfx/enterprise-guidance)
- [Use existing JavaScript libraries in SharePoint Framework client-side web parts](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/guidance/use-existing-javascript-libraries)
- [Use the Office 365 content delivery network (CDN)](https://docs.microsoft.com/sharepoint/dev/general-development/office-365-cdn)

## SharePoint Add-ins

_**Applies to:** Office 365 | SharePoint Server_

The approaches you take to ensure optimal performance with SharePoint is different in the new SharePoint Add-in model than it was with Full Trust Code. In a typical Full Trust Code (FTC) / Farm Solution scenario most code operations took place in the SharePoint Server-side Object Model code.

### Articles

- [JavaScript Patterns and Performance](https://docs.microsoft.com/sharepoint/dev/solution-guidance/javascript-patterns-and-performance)
- [Performance considerations in the SharePoint Add-in model](https://docs.microsoft.com/sharepoint/dev/solution-guidance/performance-considerations-sharepoint-add-in)
- [Improve performance in SharePoint provider-hosted add-ins](https://docs.microsoft.com/sharepoint/dev/solution-guidance/improve-performance-in-sharepoint-provider-hosted-add-ins)
- [Make batch requests with the REST APIs](https://docs.microsoft.com/sharepoint/dev/sp-add-ins/make-batch-requests-with-the-rest-apis)

### Videos

- [Office Dev PnP Web Cast – JavaScript performance considerations with SharePoint](https://developer.microsoft.com/office/blogs/javascript-performance-considerations-with-sharepoint)

### Samples

- [Caching examples](https://github.com/SharePoint/PnP/tree/master/Samples/Performance.Caching)

## Portals

_**Applies to:** Office 365 | SharePoint Server_

### Articles

- [Proven Practices for SharePoint Online Portals - Performance](https://docs.microsoft.com/sharepoint/dev/solution-guidance/portal-performance)
- [Proven Practices for SharePoint Online Portals - Navigation Solutions](https://docs.microsoft.com/sharepoint/dev/solution-guidance/portal-navigation)
- [JavaScript Patterns and Performance](https://docs.microsoft.com/sharepoint/dev/solution-guidance/javascript-patterns-and-performance)
- [Optimize page performance in SharePoint](https://docs.microsoft.com/sharepoint/dev/general-development/optimize-page-performance-in-sharepoint)

### Videos

- [Learn how to build a fast, responsive SharePoint portal in SharePoint Online](https://www.youtube.com/watch?v=tD3mkbfhIbM)
