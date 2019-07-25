---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bde44e2603ebab6be74016b16ad649918eaa7202
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872929"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageFileCountsCollectionPage getOneDriveUsageFileCounts = graphClient.reports()
    .getOneDriveUsageFileCounts('D7')
    .buildRequest()
    .get();

```