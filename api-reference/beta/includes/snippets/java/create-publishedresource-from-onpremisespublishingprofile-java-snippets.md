---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4904c390541a0626cafe71a640be7ef375da74e5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = new PublishedResource();
publishedResource.displayName = "New provisioning";
publishedResource.resourceName = "domain1.contoso.com";

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources()
    .buildRequest()
    .post(publishedResource);

```