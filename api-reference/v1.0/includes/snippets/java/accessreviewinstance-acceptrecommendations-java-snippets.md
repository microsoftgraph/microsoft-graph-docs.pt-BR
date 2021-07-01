---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70df42426d6d251bb15f904620d634aa9df1dee7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208156"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("1234fba0-cbf0-5678-8868-0810c7f91006")
    .acceptRecommendations()
    .buildRequest()
    .post();

```