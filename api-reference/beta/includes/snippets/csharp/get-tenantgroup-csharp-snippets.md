---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8eeb098f8a18523e32cffa719b5446d9f3482fb9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroup = await graphClient.TenantRelationships.ManagedTenants.TenantGroups["{managedTenants.tenantGroup-id}"]
    .Request()
    .GetAsync();

```