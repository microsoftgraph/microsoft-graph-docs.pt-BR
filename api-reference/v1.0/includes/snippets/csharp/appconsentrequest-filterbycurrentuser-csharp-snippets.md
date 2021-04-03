---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a132b0b5ce0c0fb847e1eec48dc0ac0476deb484
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .FilterByCurrentUser(On.Reviewer)
    .Request()
    .Filter("userConsentRequests/any(u:u/status eq 'InProgress')")
    .GetAsync();

```