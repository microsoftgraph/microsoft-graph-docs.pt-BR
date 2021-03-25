---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0cc3689d6363a5ef2fa9f01a9a621f2ebf4eb3a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"]
    .Request()
    .Filter("userConsentRequests/any(u:u/status eq 'InProgress')")
    .GetAsync();

```