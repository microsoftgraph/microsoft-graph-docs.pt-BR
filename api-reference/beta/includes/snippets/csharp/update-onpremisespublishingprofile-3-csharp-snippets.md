---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6042a1ef4f18bcac0ad4ac015e8cc2587abb82c3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration
{
    AllowUpdateConfigurationOverride = false
};

var onPremisesPublishingProfiles = new OnPremisesPublishingProfile();
onPremisesPublishingProfiles.HybridAgentUpdaterConfiguration = hybridAgentUpdaterConfiguration;

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"]
    .Request()
    .UpdateAsync(onPremisesPublishingProfiles);

```