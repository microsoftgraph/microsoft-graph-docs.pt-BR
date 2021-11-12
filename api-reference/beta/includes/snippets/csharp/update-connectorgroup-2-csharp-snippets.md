---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1676a0bf097fb4fae3191c6c1e6527fbd9421ec4e31dcf6580f286a69b887c96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156257"
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