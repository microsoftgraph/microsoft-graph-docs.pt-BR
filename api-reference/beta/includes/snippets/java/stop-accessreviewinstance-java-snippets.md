---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0712d01f52afbde523eb8d32f368ea96f2a995e63311f5e73c2b84e507ce2f42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099802"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("2b83cc42-09db-46f6-8c6e-16fec466a82d").instances("61a617dd-238f-4037-8fa5-d800e515f5bc")
    .stop()
    .buildRequest()
    .post();

```