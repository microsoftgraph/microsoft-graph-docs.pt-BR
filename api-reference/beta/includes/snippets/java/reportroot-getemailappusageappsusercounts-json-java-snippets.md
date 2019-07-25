---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c242920478679fb438d0308350d7a98fe6fe229f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873928"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageAppsUserCountsCollectionPage getEmailAppUsageAppsUserCounts = graphClient.reports()
    .getEmailAppUsageAppsUserCounts('D7')
    .buildRequest()
    .get();

```