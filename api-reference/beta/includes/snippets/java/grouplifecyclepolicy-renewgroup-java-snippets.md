---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce2a23dd02f0c82ce5ec4bc443c241a0d1501648
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857749"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";

graphClient.groupLifecyclePolicies()
    .renewGroup(groupId)
    .buildRequest()
    .post();

```