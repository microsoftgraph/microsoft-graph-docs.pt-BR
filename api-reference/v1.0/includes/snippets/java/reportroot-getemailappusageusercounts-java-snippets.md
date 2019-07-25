---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 423dfc52a01d9de612c324ab1b4008f705eb39d6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886375"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageUserCounts('D7')
    .buildRequest()
    .get();

```