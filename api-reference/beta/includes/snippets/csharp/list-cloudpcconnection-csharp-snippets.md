---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 409dff697077ccf66542e05c6c061515c25ff181
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcConnections = await graphClient.TenantRelationships.ManagedTenants.CloudPcConnections
    .Request()
    .GetAsync();

```