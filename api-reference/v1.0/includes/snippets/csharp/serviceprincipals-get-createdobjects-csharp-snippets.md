---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd8794aeb8f0afae26e7eff5a796324127989ba3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.ServicePrincipals["{servicePrincipal-id}"].CreatedObjects
    .Request()
    .GetAsync();

```