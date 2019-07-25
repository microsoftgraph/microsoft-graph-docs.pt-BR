---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9a81d5ae8ecb56918e47810d60b38b678b1bdbb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884650"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityFileCounts('D7')
    .buildRequest()
    .get();

```