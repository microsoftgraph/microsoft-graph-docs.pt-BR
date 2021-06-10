---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b72df6deefcf972f41fa6bd9d28a0a8a052afab5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```