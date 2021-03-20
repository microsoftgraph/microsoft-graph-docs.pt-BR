---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 457083d824759960e9197066eb8bb6ceed502fbe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewCollectionPage accessReviews = graphClient.accessReviews()
    .buildRequest()
    .filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .skip(0)
    .top(100)
    .get();

```