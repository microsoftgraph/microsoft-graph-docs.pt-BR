---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 309b4c58750ae33bb92165d80bf4cad1e1f720b7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891433"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityUserCounts('D7')
    .buildRequest()
    .get();

```