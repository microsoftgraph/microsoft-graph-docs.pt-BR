---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f85bc90847f80b6968ca44dd85411a8a0e2f1c25
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("2b83cc42-09db-46f6-8c6e-16fec466a82d").instances("61a617dd-238f-4037-8fa5-d800e515f5bc")
    .stop()
    .buildRequest()
    .post();

```