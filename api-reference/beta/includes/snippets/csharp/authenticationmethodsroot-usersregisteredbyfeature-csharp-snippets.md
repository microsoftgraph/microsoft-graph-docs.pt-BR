---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3ed49c427ad24073e02c54c8b5b2217cbbc6f00
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationFeatureSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByFeature(.all,.all)
    .Request()
    .GetAsync();

```