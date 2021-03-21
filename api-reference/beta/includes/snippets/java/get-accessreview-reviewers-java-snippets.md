---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74253fb26db7add0b3332e99d006d9294fc44428
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewReviewerCollectionPage reviewers = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers()
    .buildRequest()
    .get();

```