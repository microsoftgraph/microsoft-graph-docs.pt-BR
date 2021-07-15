---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa5e4601c573366cd3771d40131f584a9b03cc62
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceCompliance = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceCompliances["{managedTenants.managedDeviceCompliance-id}"]
    .Request()
    .GetAsync();

```