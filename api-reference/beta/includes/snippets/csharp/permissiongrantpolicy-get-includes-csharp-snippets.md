---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e87c3ce8df7e01b4a1b015c0d48fd1e019ce0cd2
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includes = await graphClient.Policies.PermissionGrantPolicies["microsoft-application-admin"].Includes
    .Request()
    .GetAsync();

```