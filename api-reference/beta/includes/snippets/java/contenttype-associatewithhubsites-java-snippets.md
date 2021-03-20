---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b5d1f5f06977519fa80d4400c5b258688f7d7b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> hubSiteUrlsList = new LinkedList<String>();
hubSiteUrlsList.add("https://graph.microsoft.com/beta/sites/id");

Boolean propagateToExistingLists = false;

graphClient.sites("id").contentTypes("id")
    .associateWithHubSites(ContentTypeAssociateWithHubSitesParameterSet
        .newBuilder()
        .withHubSiteUrls(hubSiteUrlsList)
        .withPropagateToExistingLists(propagateToExistingLists)
        .build())
    .buildRequest()
    .post();

```