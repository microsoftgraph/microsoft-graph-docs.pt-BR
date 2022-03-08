---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79e4f694de0a7cfff7ad85a2ee52c9565103993e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyServicePrincipals = await graphClient.IdentityProtection.RiskyServicePrincipals
    .Request()
    .GetAsync();

```