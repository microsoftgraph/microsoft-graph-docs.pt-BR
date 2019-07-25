---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c2b0a191feb12a103688ca83067209a182c62af
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872137"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityUserCountsCollectionPage getSkypeForBusinessOrganizerActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityUserCounts('D7')
    .buildRequest()
    .get();

```