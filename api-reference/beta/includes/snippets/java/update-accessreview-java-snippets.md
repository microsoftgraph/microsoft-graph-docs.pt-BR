---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a773bca708ec21f3fed3507b1cb03526ce5105fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972823"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = new AccessReview();
accessReview.displayName = "TestReview new name";

graphClient.accessReviews("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .patch(accessReview);

```