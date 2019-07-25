---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66a579ce73d90e002498359793262f8aece85e45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872101"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityCountsCollectionPage getSkypeForBusinessParticipantActivityCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityCounts('D7')
    .buildRequest()
    .get();

```