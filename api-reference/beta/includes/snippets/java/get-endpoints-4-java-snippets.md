---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 727e46bd38a1a0d8711a1dfaec22e3cea8242a22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953059"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByUserCollectionPage dailyPrintUsageSummariesByUser = graphClient.print().reports().dailyPrintUsageSummariesByUser()
    .buildRequest()
    .get();

```