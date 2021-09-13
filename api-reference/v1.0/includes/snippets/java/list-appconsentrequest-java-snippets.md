---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c44196b4af7295a1aab1a7ddc040fc8eea884efb28b4450d07e2e81003f0ada4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequestCollectionPage appConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests()
    .buildRequest()
    .get();

```