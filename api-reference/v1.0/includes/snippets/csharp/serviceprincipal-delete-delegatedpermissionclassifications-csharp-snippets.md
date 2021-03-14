---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71cbbd426209b160d82b17860b9adc07bcbd5b39
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].DelegatedPermissionClassifications["{delegatedPermissionClassification-id}"]
    .Request()
    .DeleteAsync();

```