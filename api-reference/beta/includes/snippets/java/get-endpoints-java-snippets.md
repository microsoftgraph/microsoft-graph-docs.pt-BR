---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7eca49c98e0fe203933bd0aac5740f46312f1be
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015361"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRoot reportRoot = graphClient.print().reports("dailyPrintUsageSummariesByPrinter")
    .buildRequest()
    .get();

```