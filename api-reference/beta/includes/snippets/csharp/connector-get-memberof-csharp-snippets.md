---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b34c509f6ad5072fe2e861765bfd1f15ccb8120e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"].MemberOf
    .Request()
    .GetAsync();

```