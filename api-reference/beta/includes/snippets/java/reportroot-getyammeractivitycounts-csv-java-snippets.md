---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8cfd8d37a749b95fd8671f4de87878020180e96
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivitySummaryCollectionPage getYammerActivityCounts = graphClient.reports()
    .getYammerActivityCounts('D7')
    .buildRequest()
    .get();

```