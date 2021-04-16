---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 995312bd284c5e68d82e14caa377227a0b5d9bcc
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51837821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .FilterByCurrentUser(ConsentRequestFilterByCurrentUserOptions.Reviewer)
    .Request()
    .Filter(" (status eq 'Completed')")
    .GetAsync();

```