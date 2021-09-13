---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1161e823592c406f633f9d9b8e7234333dcfb7a6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hubSiteUrls = new List<String>()
{
    "https://graph.microsoft.com/v1.0/sites/{site-id}"
};

var propagateToExistingLists = false;

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .AssociateWithHubSites(hubSiteUrls,propagateToExistingLists)
    .Request()
    .PostAsync();

```