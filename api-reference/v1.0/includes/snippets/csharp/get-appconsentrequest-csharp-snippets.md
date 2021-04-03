---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9783bdc13de215622451af197a2d465fb3a03efd
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"]
    .Request()
    .GetAsync();

```