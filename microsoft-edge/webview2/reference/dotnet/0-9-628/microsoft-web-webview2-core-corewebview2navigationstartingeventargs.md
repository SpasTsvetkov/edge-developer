---
description: Embed web technologies (HTML, CSS, and JavaScript) in your native applications with the Microsoft Edge WebView2 control
title: Microsoft.Web.WebView2.Core.CoreWebView2NavigationStartingEventArgs
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/10/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: Microsoft.Web.WebView2, Core, webview2, webview, dotnet, wpf, winforms, app, edge, CoreWebView2, CoreWebView2Controller, browser control, edge html, Microsoft.Web.WebView2.Core.CoreWebView2NavigationStartingEventArgs
---

# Microsoft.Web.WebView2.Core.CoreWebView2NavigationStartingEventArgs class 

Namespace: Microsoft.Web.WebView2.Core\
Assembly: Microsoft.Web.WebView2.Core.dll

Event args for the NavigationStarting event.

## Summary

 Members                        | Descriptions
--------------------------------|---------------------------------------------
[Cancel](#cancel) | The host may set this flag to cancel the navigation.
[IsRedirected](#isredirected) | True when the navigation is redirected.
[IsUserInitiated](#isuserinitiated) | True when the navigation was initiated through a user gesture as opposed to programmatic navigation.
[NavigationId](#navigationid) | The ID of the navigation.
[RequestHeaders](#requestheaders) | The HTTP request headers for the navigation.
[Uri](#uri) | The uri of the requested navigation.

## Members

#### Cancel 

The host may set this flag to cancel the navigation.

> public bool [Cancel](#cancel)

If set, it will be as if the navigation never happened and the current page's content will be intact. For performance reasons, GET HTTP requests may happen, while the host is responding. This means cookies can be set and used part of a request for the navigation.

#### IsRedirected 

True when the navigation is redirected.

> public bool [IsRedirected](#isredirected)

#### IsUserInitiated 

True when the navigation was initiated through a user gesture as opposed to programmatic navigation.

> public bool [IsUserInitiated](#isuserinitiated)

#### NavigationId 

The ID of the navigation.

> public ulong [NavigationId](#navigationid)

#### RequestHeaders 

The HTTP request headers for the navigation.

> public CoreWebView2HttpRequestHeaders [RequestHeaders](#requestheaders)

Note, you cannot modify the HTTP request headers in a NavigationStarting event.

#### Uri 

The uri of the requested navigation.

> public string [Uri](#uri)

