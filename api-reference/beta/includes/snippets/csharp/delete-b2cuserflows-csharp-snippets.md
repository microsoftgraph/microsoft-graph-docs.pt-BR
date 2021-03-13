---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2946fbadecadb1ee9c34871db93dffe0cd23717b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```