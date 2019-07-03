---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3debe5217c9da100fb7d53bbd05722f7ae47a227
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityRiskEvents = await graphClient.IdentityRiskEvents
    .Request()
    .GetAsync();

```