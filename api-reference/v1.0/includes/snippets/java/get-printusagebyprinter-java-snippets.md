---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83bc6146199fa0b8d6bc3851877c4c361e93b0bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774451"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.reports().dailyPrintUsageByPrinter("{id}")
    .buildRequest()
    .get();

```