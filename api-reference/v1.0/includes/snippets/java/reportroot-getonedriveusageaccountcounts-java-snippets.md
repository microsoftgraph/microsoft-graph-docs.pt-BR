---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 926df651377f5c6fc5ae04b7d49a13cb64b93847
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327591"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageAccountCounts("D7")
    .buildRequest()
    .get();

```