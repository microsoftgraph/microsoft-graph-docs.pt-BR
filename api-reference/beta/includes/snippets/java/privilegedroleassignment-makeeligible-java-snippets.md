---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54539e9654cbe414cc92c696af91e2d94f87bb05
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875690"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignments("{id}")
    .makeEligible()
    .buildRequest()
    .post();

```