---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcb87c3b0603a5d7fd0430213bef7f5269b82c66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954245"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByUserCollectionPage monthlyPrintUsageSummariesByUser = graphClient.print().reports().monthlyPrintUsageSummariesByUser()
    .buildRequest()
    .get();

```