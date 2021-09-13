---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35870ce3bf012b5d131a7ae76bdbe140d384336bce6f26b830c58c0d2858e4ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329212"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequest appConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("af330b30-dd59-4482-a848-0fd81b0438ed")
    .buildRequest()
    .get();

```