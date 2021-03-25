---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79d7f1c821e74db86e1c99f05f10ec29612691d9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequestCollectionPage appConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests()
    .buildRequest()
    .filter("userConsentRequests/any (u:u/status eq 'InProgress')")
    .get();

```