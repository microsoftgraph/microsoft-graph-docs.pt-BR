---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 957a3b68bc5233ba7402e67c1bea9d9b616c5a20
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873015"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageAccountCountsCollectionPage getOneDriveUsageAccountCounts = graphClient.reports()
    .getOneDriveUsageAccountCounts('D7')
    .buildRequest()
    .get();

```