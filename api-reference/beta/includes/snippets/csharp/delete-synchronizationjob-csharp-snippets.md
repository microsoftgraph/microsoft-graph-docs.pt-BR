---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5b760820b507bf53c7b082cd2009d7ca6a2af7b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Request()
    .DeleteAsync();

```