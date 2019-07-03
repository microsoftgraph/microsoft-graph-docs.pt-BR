---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1f77c5ea2102b0cc5ae408aa8f92dd05a4a1365
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```