---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85cebc3979ec52bf1f302a846e29b3ffb356ee98
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications["{id}"]
    .Request()
    .DeleteAsync();

```