---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 534b9b670e3357bfbc774291c83f712d51c4d012
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDevice = await graphClient.TenantRelationships.ManagedTenants.CloudPcDevices["{managedTenants.cloudPcDevice-id}"]
    .Request()
    .GetAsync();

```