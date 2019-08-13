---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53784f93374b22b444073b3b513133ec5132127b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308748"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "feature eq 'registration'"));

ICredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
    .getCredentialUsageSummary("D30")
    .buildRequest( requestOptions )
    .get();

```