---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7870c02af59fe76d53d4ca04686d3f6b3457b273
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"].Members
    .Request()
    .GetAsync();

```