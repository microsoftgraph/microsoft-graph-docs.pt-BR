---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4971c7221423f9f0c1d65e848b3962d4fe9107f9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210634"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage monthlyPrintUsageByPrinter = graphClient.reports().monthlyPrintUsageByPrinter()
    .buildRequest()
    .get();

```