---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3868516361a0f72f32a0112dae2d872015e4fc71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874986"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = new PublishedResource();
publishedResource.displayName = "Demo provisioning (updated)";

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("1234b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .patch(publishedResource);

```