---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78529d8c9a1915eb0373dcc49e25ccf6662ae44d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358626"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivitySummaryCollectionPage getYammerActivityUserCounts = graphClient.reports()
    .getYammerActivityUserCounts("D7")
    .buildRequest()
    .get();

```