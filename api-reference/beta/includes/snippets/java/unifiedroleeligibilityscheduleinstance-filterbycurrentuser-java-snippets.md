---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90e719c4938ed58f1c25cac6e7423ee9dfd498d6
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514747"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstanceFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleEligibilityScheduleInstances()
    .filterByCurrentUser(UnifiedRoleEligibilityScheduleInstanceFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```