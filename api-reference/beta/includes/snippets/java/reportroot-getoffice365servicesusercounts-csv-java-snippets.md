---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9981b4f8d8d3e7a481ba3dcde0374238532698db
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873215"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ServicesUserCountsCollectionPage getOffice365ServicesUserCounts = graphClient.reports()
    .getOffice365ServicesUserCounts('D7')
    .buildRequest()
    .get();

```