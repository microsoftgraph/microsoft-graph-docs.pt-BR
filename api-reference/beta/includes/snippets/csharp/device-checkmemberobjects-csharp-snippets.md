---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5540bf65265855088aa1e43e6c1449fd90193d82
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
};

await graphClient.Devices["{id}"]
    .CheckMemberObjects(ids)
    .Request()
    .PostAsync();

```