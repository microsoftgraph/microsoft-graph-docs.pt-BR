---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7f760b225fd25bda62cc9bf1d4668db40f969b158e7215b08a67f156c301ed2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214301"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.reports().dailyPrintUsageByPrinter("{id}")
    .buildRequest()
    .get();

```