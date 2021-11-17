---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5a74c2b6099feef8a9a7dc01418444871b21ddd45462494f712bbd9accfb071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcConnection = await graphClient.TenantRelationships.ManagedTenants.CloudPcConnections["{managedTenants.cloudPcConnection-id}"]
    .Request()
    .GetAsync();

```