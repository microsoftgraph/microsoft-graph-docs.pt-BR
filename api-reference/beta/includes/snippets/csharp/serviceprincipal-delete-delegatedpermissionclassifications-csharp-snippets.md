---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85cebc3979ec52bf1f302a846e29b3ffb356ee98
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458598"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications["{id}"]
    .Request()
    .DeleteAsync();

```