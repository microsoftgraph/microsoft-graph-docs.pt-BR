---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91233164e89985e697d913308b2c91caadf2ffd7ef76b26e6b6e8d12deaaa7c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementIntent = await graphClient.TenantRelationships.ManagedTenants.ManagementIntents["{managedTenants.managementIntent-id}"]
    .Request()
    .GetAsync();

```