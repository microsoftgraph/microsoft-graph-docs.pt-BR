---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53e54ad6356b170b01ab1676df43cd2314f5d519
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "All Contoso volunteers - Terms of use";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.identityGovernance().termsOfUse().agreements("0ec9f6a6-159d-4dd8-a563-1f0b5935e80b")
    .buildRequest()
    .patch(agreement);

```