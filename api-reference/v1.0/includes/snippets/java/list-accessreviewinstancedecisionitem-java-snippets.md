---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b4fa903dfa45a99d58c93c23cfdc9b3b4fda3e3052eaeea8b7b79fa5c8aa87c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158157"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("2dca8959-b716-4b4c-a93d-a535c01eb6e0").instances("8d035c9d-798d-47fa-beb4-f986a4b8126f").decisions()
    .buildRequest()
    .get();

```