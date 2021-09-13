---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589d64a003c69c1befd671dc4b3931a915f8fa291b3f0c19cc1c9f61004709d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274598"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .FilterByCurrentUser(ConsentRequestFilterByCurrentUserOptions.Reviewer)
    .Request()
    .Filter("userConsentRequests/any(u:u/status eq 'InProgress')")
    .GetAsync();

```