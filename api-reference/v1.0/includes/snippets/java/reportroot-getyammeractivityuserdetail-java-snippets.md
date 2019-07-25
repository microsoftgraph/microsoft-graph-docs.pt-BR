---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0962c482f9a719e37e2df18926fa5f25dc10569
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881026"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityUserDetail('D7')
    .buildRequest()
    .get();

```