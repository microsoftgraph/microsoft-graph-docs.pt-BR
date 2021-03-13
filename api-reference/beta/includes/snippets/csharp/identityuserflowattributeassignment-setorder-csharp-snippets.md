---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54c57653327b2fdfd16c74208aa2fddd276cb756
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newAssignmentOrder = new AssignmentOrder
{
    Order = new List<String>()
    {
        "City",
        "extension_GUID_ShoeSize"
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .SetOrder(newAssignmentOrder)
    .Request()
    .PostAsync();

```