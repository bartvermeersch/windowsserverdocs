---
title: bitsadmin setcustomheaders
description: Windows Commands topic for **bitsadmin setcustomheaders**, which adds a custom HTTP header to a GET request.
ms.prod: windows-server
ms.technology: manage-windows-commands
ms.topic: article
ms.assetid: ed926410-80d0-46ed-9a90-f752c164bb9a
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017 
---

# bitsadmin setcustomheaders

Add a custom HTTP header to a GET request sent to an HTTP server.

## Syntax

```
bitsadmin /setcustomheaders <job> <header1> <header2> <...>
```

### Parameters

| Parameter | Description |
| --------- | ----------- |
| job | The job's display name or GUID. |
| `<header1> <header2>` and so on | The custom headers for the job. |

## Examples

The following example adds a custom HTTP header for the job named *myDownloadJob*. For more information about GET requests, see [Method Definitions](https://www.w3.org/Protocols/rfc2616/rfc2616-sec9.html#sec9.3) and [Header Field Definitions](https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html).

```
C:\>bitsadmin /setcustomheaders myDownloadJob accept-encoding:deflate/gzip
```

## Additional References

- [Command-Line Syntax Key](command-line-syntax-key.md)