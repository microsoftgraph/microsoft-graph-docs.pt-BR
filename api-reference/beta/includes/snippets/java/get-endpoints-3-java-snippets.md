---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 866f5448b4ad04fec21925188c7abd58338830fd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211000"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage dailyPrintUsageSummariesByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter()
    .buildRequest()
    .get();

```