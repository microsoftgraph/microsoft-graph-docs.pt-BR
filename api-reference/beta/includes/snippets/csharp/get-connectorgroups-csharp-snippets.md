---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a42bfd2155ad86979247ea7cff3da5896f522ab309030e3dda164bc37b524b86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroups = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups
    .Request()
    .GetAsync();

```