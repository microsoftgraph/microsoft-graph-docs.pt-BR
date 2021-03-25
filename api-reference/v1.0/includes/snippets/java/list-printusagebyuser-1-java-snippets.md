---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 420b5319a8399265a854ca405325aaa6d97f7353
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208183"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage dailyPrintUsageByUser = graphClient.reports().dailyPrintUsageByUser()
    .buildRequest()
    .get();

```