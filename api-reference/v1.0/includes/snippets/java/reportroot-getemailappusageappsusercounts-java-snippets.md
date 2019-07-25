---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ced4dc2c59be903effaec1d0e0765b698fca5019
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891883"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageAppsUserCounts('D7')
    .buildRequest()
    .get();

```