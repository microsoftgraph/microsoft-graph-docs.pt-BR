---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 221b9ffb697adf90fded2cbbfc754ddd2ec58fd8454501e2b2493dc7661bd7b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests["{unifiedRoleEligibilityScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```