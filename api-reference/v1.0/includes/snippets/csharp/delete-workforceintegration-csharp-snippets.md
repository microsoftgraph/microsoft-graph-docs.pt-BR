---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7adefadd86121453bd3645a0cc3870dcba6b0b3a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.WorkforceIntegrations["{workforceIntegration-id}"]
    .Request()
    .DeleteAsync();

```