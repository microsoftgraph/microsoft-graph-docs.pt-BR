---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3506a457a1b97de499edbeada7d3cac2976804c
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorReference = new ReferenceRequestBody
{
    ODataId = "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"].Members.References
    .Request()
    .AddAsync(connectorReference);

```