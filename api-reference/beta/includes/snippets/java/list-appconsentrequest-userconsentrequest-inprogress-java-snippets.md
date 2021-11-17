---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6990d86dff5f26c0174d08e2267a5988f27decdff0aa2641acb7cd2508d648a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequestCollectionPage appConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests()
    .buildRequest()
    .filter("userConsentRequests/any (u:u/status eq 'InProgress')")
    .get();

```