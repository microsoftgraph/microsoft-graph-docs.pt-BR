---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4acfc3282ff104ed0e0ba4a3cfac6365e8b1c0c8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .Request()
    .GetAsync();

```