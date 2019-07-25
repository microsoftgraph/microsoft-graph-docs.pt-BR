---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9370c7ba52aa20895de9125656c008620c901c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873785"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageVersionsUserCountsCollectionPage getEmailAppUsageVersionsUserCounts = graphClient.reports()
    .getEmailAppUsageVersionsUserCounts('D7')
    .buildRequest()
    .get();

```