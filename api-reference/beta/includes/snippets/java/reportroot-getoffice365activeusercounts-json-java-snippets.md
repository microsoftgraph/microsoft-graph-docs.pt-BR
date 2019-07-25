---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5395c3382c9c77af0b57cbb51b5dccefa95e6487
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872869"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActiveUserCountsCollectionPage getOffice365ActiveUserCounts = graphClient.reports()
    .getOffice365ActiveUserCounts('D7')
    .buildRequest()
    .get();

```