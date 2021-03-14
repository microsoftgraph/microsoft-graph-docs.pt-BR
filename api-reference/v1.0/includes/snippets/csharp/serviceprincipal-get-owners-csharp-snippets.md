---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f59da63b2564eb5fea59b0ded08bb7ba29874e2d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners
    .Request()
    .GetAsync();

```