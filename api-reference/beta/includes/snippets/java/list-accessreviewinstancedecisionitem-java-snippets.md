---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b389713a9fdc43b43d657d7e9ce336b53cbea1d8f04c18cd3fc7f64706fce84a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("16d424f6-0100-4bf1-9ebc-fe009c5e5006").instances("bb14c722-51b8-4962-9bd2-1d96ba773d80").decisions()
    .buildRequest()
    .get();

```