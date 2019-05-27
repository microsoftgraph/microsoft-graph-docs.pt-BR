---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8803e13de770f6c692ef0da4cb605774cbc26ce0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```