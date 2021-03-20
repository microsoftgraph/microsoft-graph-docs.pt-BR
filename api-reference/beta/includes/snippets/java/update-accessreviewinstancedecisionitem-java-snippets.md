---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 478d1e7881bcec170e3b3c1c9b0b9f51a550fa07
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973578"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem();
accessReviewInstanceDecisionItem.decision = "Approve";
accessReviewInstanceDecisionItem.justification = "I trust this person";

graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19").decisions("654b34e7-b48f-4772-a2d4-08f1d0dd014c")
    .buildRequest()
    .patch(accessReviewInstanceDecisionItem);

```