---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 126c756bd90b9afa1713362a531c7c78b3155ada6b1c9c4ff5ceb7a455bd9632
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"].Members
    .Request()
    .GetAsync();

```