---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0f34b90f48d60dd9618e04feabe1727d63e430a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095196"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSet ediscoveryReviewSet = new EdiscoveryReviewSet();
ediscoveryReviewSet.displayName = "My review set 2";

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").reviewSets()
    .buildRequest()
    .post(ediscoveryReviewSet);

```