---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52f2785c2d031a6963d19b2ca554ab0c56a8068aca08c704a0156109de734995
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214076"
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