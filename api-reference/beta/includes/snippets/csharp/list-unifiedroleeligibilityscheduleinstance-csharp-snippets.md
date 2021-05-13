---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c085117ee28f5bed0ccba2f8edf7e96c8c139acc
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilityScheduleInstances = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances
    .Request()
    .GetAsync();

```