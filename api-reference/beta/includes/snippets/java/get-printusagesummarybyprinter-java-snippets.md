---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4ea549b11fc8a00d9dd07a3fcb4b55db73361ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967101"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter("{id}")
    .buildRequest()
    .get();

```