---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10285f1bede934bd262ca3dcfdff5adc6bb93fa4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240985"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = graphClient.identityGovernance().accessReviews().policy()
    .buildRequest()
    .get();

```