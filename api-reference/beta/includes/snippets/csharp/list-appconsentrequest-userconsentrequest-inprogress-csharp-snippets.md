---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 662705f66e6c63b7bf03c865e57f682e8af63153
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .Request()
    .Filter("userConsentRequests/any (u:u/status eq 'InProgress')")
    .GetAsync();

```