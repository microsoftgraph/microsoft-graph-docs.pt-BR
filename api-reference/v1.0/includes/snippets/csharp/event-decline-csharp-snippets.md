---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b51f7858ee54c5c7103444f112a56fa3b552375d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Decline(comment,sendResponse)
    .Request()
    .PostAsync();

```