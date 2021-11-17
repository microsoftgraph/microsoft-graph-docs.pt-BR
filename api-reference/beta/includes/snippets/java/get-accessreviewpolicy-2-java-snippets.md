---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2857efe3ef3d89451308c2b6b8393870e3398321fd5f0bf123f410954d7a269a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898164"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = graphClient.identityGovernance().accessReviews().policy()
    .buildRequest()
    .get();

```