---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16ca88bd996dd8795475e8d5e43948ab989616b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318647"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationSignInSummaryCollectionPage getAzureADApplicationSignInSummary = graphClient.reports()
    .getAzureADApplicationSignInSummary("D7")
    .buildRequest()
    .get();

```