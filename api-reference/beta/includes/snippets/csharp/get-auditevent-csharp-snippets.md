---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6cfd064fef73599b1e5cf7c96f3067525453901
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditEvent = await graphClient.TenantRelationships.ManagedTenants.AuditEvent
    .Request()
    .GetAsync();

```