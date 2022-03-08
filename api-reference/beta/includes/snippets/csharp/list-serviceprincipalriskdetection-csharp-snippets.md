---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed963ee3644b51e0ebd8947e49308f6a59fd09b7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipalRiskDetections = await graphClient.IdentityProtection.ServicePrincipalRiskDetections
    .Request()
    .GetAsync();

```