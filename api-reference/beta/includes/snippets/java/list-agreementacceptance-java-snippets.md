---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b4503b14e32a1453588cfe013b052292fb44343
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516158"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementAcceptanceCollectionPage acceptances = graphClient.identityGovernance().termsOfUse().agreements("94410bbf-3d3e-4683-8149-f034e55c39dd").acceptances()
    .buildRequest()
    .get();

```