---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffdf769f011e36e7e16ef407ed324d1ca2369ca7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855487"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "displayName-value";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.agreements("'id'")
    .buildRequest()
    .patch(agreement);

```