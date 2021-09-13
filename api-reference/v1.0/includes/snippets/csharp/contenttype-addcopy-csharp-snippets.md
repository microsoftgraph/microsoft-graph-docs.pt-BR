---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e43e17b72beb2fa4b4b562a051a75b0b3995aeb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopy(contentType)
    .Request()
    .PostAsync();

```