---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 995da2f9b786e790f0e3fc91250ff4dc8074b64e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856048"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d")
    .buildRequest()
    .get();

```