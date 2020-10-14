---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 068488d8c730a8e5c8148f8f9ecfee2f7061bb93
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassifications = await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications
    .Request()
    .GetAsync();

```