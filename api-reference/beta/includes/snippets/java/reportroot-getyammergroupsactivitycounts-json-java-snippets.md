---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2960c0df9a8cd334c5800102e8b9f9c8a715992f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityCountsCollectionPage getYammerGroupsActivityCounts = graphClient.reports()
    .getYammerGroupsActivityCounts('D7')
    .buildRequest()
    .get();

```