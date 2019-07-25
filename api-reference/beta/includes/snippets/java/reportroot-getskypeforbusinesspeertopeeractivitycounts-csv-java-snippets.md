---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 174e3a9135357d0575f3fca0f4b53e4c8bff53c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871954"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityCountsCollectionPage getSkypeForBusinessPeerToPeerActivityCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityCounts('D7')
    .buildRequest()
    .get();

```