---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e74fed728b73e3c7044eca7718c2c6caefc62c79
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.IdentityProtection.RiskyServicePrincipals["{riskyServicePrincipal-id}"].History
    .Request()
    .GetAsync();

```