---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23bd89e4ce9ddf610543c4df17c598d5b39e9438
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "name-value",
    Region = ConnectorGroupRegion.Nam
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"]
    .Request()
    .UpdateAsync(connectorGroup);

```