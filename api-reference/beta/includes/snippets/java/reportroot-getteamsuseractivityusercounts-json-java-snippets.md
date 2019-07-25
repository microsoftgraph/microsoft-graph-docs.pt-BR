---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de62dac41bc577d4c2411c4cb30149cf040d2add
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871682"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityUserCountsCollectionPage getTeamsUserActivityUserCounts = graphClient.reports()
    .getTeamsUserActivityUserCounts('D7')
    .buildRequest()
    .get();

```