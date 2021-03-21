---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9cc87b1a6759cf31ab26c2be42da727f1dc3af2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978110"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = new PublishedResource();
publishedResource.displayName = "Demo provisioning (updated)";

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("1234b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .patch(publishedResource);

```