---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 631e1e9d3e6bdc29c8d5ef85c0185c746d92dee3
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilitySchedules = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules
    .Request()
    .GetAsync();

```