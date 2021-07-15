---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e50d124efa7405583a75e49162ae33ad0e683306
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsProtectionState = await graphClient.TenantRelationships.ManagedTenants.WindowsProtectionStates["{managedTenants.windowsProtectionState-id}"]
    .Request()
    .GetAsync();

```