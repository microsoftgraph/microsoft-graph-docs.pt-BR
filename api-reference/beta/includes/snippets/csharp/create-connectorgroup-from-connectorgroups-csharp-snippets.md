---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8178b16ba4a9c495e81633fa837399665922872b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "name-value",
    IsDefault = false
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups
    .Request()
    .AddAsync(connectorGroup);

```