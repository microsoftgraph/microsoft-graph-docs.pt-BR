---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39562f12778160ad8b4dea2a7bf170668fb3c9b10bd3c59a4e07ccfd7b11bf21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("aed0b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .expand("agentGroups")
    .get();

```