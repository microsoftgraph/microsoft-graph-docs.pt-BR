---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d67e46be0be969521184e795f27f9f795547b704
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951491"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewReviewerCollectionPage reviewers = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers()
    .buildRequest()
    .get();

```