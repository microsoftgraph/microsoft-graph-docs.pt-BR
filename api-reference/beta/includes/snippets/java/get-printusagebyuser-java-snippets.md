---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f63382c19b135d242f7250055455aa7fface342
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUser printUsageByUser = graphClient.print().reports().dailyPrintUsageByUser("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
    .buildRequest()
    .get();

```