---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fd31e39f337ba854b1356c8d94fdf388a7685ab079195bc03225975e52a8990
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcConnections = await graphClient.TenantRelationships.ManagedTenants.CloudPcConnections
    .Request()
    .GetAsync();

```