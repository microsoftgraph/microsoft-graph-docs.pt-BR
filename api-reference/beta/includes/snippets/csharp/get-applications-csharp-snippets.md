---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42cb3a22ed9e91054e2e860e68002d08e2d77dfa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"].Applications
    .Request()
    .GetAsync();

```