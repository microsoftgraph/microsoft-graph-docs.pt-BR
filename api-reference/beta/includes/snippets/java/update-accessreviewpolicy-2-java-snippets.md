---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9aa2d1dbfa7a0c6e20f4424ddcf4059c028c30d265746c48dbd73861b2c2201b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = new AccessReviewPolicy();
accessReviewPolicy.isGroupOwnerManagementEnabled = true;

graphClient.identityGovernance().accessReviews().policy()
    .buildRequest()
    .patch(accessReviewPolicy);

```