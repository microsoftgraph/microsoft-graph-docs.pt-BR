---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec053dec5ba778afa0dcfab1a7c65b332332f8d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```