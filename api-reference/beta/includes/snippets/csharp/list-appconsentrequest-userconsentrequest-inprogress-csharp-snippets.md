---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e26546613e4ae40ccaa05a824a88886f7c1bfba053b77b8a2d9ef5aac374467
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .Request()
    .Filter("userConsentRequests/any (u:u/status eq 'InProgress')")
    .GetAsync();

```