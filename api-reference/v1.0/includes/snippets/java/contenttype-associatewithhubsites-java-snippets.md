---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1d24e21d7b6b5e0ff0ac62cbc613115234d3d68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147662"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> hubSiteUrlsList = new LinkedList<String>();
hubSiteUrlsList.add("https://graph.microsoft.com/v1.0/sites/{site-id}");

Boolean propagateToExistingLists = false;

graphClient.sites("{site-id}").contentTypes("{contentTypeId}")
    .associateWithHubSites(ContentTypeAssociateWithHubSitesParameterSet
        .newBuilder()
        .withHubSiteUrls(hubSiteUrlsList)
        .withPropagateToExistingLists(propagateToExistingLists)
        .build())
    .buildRequest()
    .post();

```