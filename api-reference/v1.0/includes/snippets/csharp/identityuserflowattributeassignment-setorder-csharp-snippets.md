---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40c1c660ce3d7da684ee9a5e555cce1156004edf520360a3426262494f52ee0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275157"
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

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .SetOrder(newAssignmentOrder)
    .Request()
    .PostAsync();

```