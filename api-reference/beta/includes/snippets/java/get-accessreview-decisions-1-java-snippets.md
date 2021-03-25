---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 524e842957517ed77f266670b80f9ac08b5e45ea
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewDecisionCollectionPage decisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").decisions()
    .buildRequest()
    .get();

```