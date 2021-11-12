---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf2c97366a2b8c408c154e6da2e2f2c68baca53888f70bafec460165ecbc73ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors
    .Request()
    .GetAsync();

```