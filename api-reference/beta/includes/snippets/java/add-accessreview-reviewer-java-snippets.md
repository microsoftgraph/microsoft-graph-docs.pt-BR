---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d17ccb60496beb189b5c6420a775f86129f22c83
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951729"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewReviewer accessReviewReviewer = new AccessReviewReviewer();
accessReviewReviewer.id = "006111db-0810-4494-a6df-904d368bd81b";

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers()
    .buildRequest()
    .post(accessReviewReviewer);

```