---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93f843fc24f1bd8cba04341e7784e0c161038303
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.accountEnabled = true;
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("businessPhones-value");
user.businessPhones = businessPhonesList;
user.city = "city-value";

graphClient.me()
    .buildRequest()
    .patch(user);

```