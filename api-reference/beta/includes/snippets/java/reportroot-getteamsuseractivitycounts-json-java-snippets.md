---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77dfd9395d352de9bb85fbed65d17f00c23a3be5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358761"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityCountsCollectionPage getTeamsUserActivityCounts = graphClient.reports()
    .getTeamsUserActivityCounts("D7")
    .buildRequest()
    .get();

```