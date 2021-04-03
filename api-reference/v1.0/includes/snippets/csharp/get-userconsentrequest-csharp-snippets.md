---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05c72b41873711a44904c306761e4b9f44cb0f71
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests["{userConsentRequest-id}"]
    .Request()
    .GetAsync();

```