---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9a9e0ea4642f12f8894d4d6c5ce82d216f2bec25ffa3ff7cd3b155f6af39ab1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898154"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = new AccessReviewPolicy();
accessReviewPolicy.isGroupOwnerManagementEnabled = true;

graphClient.policies().accessReviewPolicy()
    .buildRequest()
    .patch(accessReviewPolicy);

```