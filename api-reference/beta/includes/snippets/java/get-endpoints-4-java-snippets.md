---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58f601141e9aa3e0c936691a66dfe02829d191c2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209817"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage dailyPrintUsageSummariesByUser = graphClient.print().reports().dailyPrintUsageSummariesByUser()
    .buildRequest()
    .get();

```