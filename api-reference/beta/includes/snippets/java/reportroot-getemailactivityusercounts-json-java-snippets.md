---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77ae1dbda08c0aae380c7dabcb473abcbbb57ea4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308635"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivitySummaryCollectionPage getEmailActivityUserCounts = graphClient.reports()
    .getEmailActivityUserCounts("D7")
    .buildRequest()
    .get();

```