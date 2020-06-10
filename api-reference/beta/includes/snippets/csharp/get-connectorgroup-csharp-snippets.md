---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a23752aec94f97c665475ed6bb09c7f713db2cd5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681429"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"]
    .Request()
    .GetAsync();

```