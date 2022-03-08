---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c85c4c99d0753b0678f73232b2282e9528fe0bb2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicyConfigurationPartner = await graphClient.Policies.CrossTenantAccessPolicy.Partners["{crossTenantAccessPolicyConfigurationPartner-id}"]
    .Request()
    .GetAsync();

```