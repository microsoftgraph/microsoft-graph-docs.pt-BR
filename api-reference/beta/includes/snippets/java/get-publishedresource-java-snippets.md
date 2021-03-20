---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9019a46ad6395b481eb3e40eef73a7b1babf26e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973022"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("aed0b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .expand("agentGroups")
    .get();

```