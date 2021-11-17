---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9289358240f132fba82096bb0cba130646d6c8508b090eb52e5c9e8bc9293b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDevices = await graphClient.TenantRelationships.ManagedTenants.CloudPcDevices
    .Request()
    .GetAsync();

```