---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb140961d42b1dfc6b141f3009dac41e5055a52f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890763"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActiveUserCounts('D7')
    .buildRequest()
    .get();

```