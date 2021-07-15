---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c80a6db0a68a894bf597049998beb1e635d02381
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementIntent = await graphClient.TenantRelationships.ManagedTenants.ManagementIntents["{managedTenants.managementIntent-id}"]
    .Request()
    .GetAsync();

```